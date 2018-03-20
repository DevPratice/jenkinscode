pipeline {
  agent {
    node {
      label 'master'
    }
    
  }
  stages {
    stage('error') {
      steps {
        git(url: 'https://github.com/cit-latex/t1-student-maven-proj.git', branch: 'master')
      }
    }
  }
}