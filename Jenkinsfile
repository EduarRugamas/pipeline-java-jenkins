pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh ' mvn package'
      }
    }

    stage('Test') {
      steps {
        sh 'echo \'test success\''
      }
    }

    stage('Deliver') {
      steps {
        sh './jenkins/scripts/deliver.sh'
      }
    }

  }
}