pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test step'
          }
        }

        stage('Test Para') {
          steps {
            echo 'Test Para'
          }
        }

        stage('Testing') {
          steps {
            echo 'Hello'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployed Success'
        sleep 12
      }
    }

  }
}