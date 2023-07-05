pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'this is development'
      }
    }

    stage('Test') {
      steps {
        echo 'this is test stage'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'this is Build stage'
          }
        }

        stage('fixes') {
          steps {
            echo 'this is fixes stage'
          }
        }

        stage('Operate') {
          steps {
            echo 'this is operate'
          }
        }

        stage('Prod') {
          steps {
            echo 'this is prod stage'
          }
        }

        stage('Deploy') {
          steps {
            echo 'This is Deployment'
          }
        }

      }
    }

  }
}