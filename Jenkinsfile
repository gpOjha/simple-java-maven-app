pipeline {
  agent any
  stages {
    stage('Commit stage') {
      steps {
        echo 'Hi this is commit stage'
      }
    }

    stage('Build stage') {
      steps {
        echo 'Hi this is build stage'
      }
    }

    stage('Test stage') {
      steps {
        echo 'Hi this is test stage'
      }
    }

    stage('Staging') {
      steps {
        echo 'Hi this is staging'
      }
    }

    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'Hi this is deploy'
          }
        }

        stage('Operate') {
          steps {
            echo 'Hi this is operate'
          }
        }

      }
    }

  }
}