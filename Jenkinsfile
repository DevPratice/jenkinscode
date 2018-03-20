pipeline {
  agent any
  stages {
    stage('Shell Commands') {
      steps {
        sh 'echo Hello World - Stage1 step1'
        sh 'echo Hello Stage1 Step2'
      }
    }
    stage('Some commands') {
      steps {
        sh 'echo some thing'
      }
    }
  }
}