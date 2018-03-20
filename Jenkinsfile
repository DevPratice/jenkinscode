pipeline {
  agent {
    node {
      label 'master'
    }
    
  }
  stages {
    stage('Git Repo') {
      steps {
        git(url: 'https://github.com/cit-latex/t1-student-maven-proj.git', branch: 'master')
      }
    }
    stage('Maven Compile') {
      steps {
        sh 'mvn compile package'
      }
    }
    stage('Upload Artifacts') {
      steps {
        sh 'mvn deploy'
      }
    }
    stage('Ansible-Deploy') {
      steps {
        sh 'ansible --version'
      }
    }
  }
}