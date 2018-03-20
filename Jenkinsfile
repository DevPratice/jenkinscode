pipeline {
  agent {
    node {
      label 'master'
    }
    
  }
  stages {
    stage('Git Clone') {
      agent {
        node {
          label 'MAVEN'
        }
        
      }
      steps {
        git(url: 'https://github.com/cit-latex/t1-student-maven-proj.git', branch: 'master')
      }
    }
    stage('Maven Compile') {
      agent {
        node {
          label 'MAVEN'
        }
        
      }
      steps {
        sh 'mvn compile package'
      }
    }
  }
}