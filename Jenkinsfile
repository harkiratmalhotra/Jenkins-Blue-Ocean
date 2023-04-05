pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'pwd'
        sh 'date'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'teststep'
          }
        }

        stage('Integration Test') {
          steps {
            echo 'Integration Test'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying the app'
      }
    }

  }
}