pipeline {
  agent any
  stages {
    stage('Development') {
      steps {
        echo 'i want to develop'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'I want to build'
          }
        }

        stage('test') {
          steps {
            echo 'I want to test'
          }
        }

        stage('deploy') {
          steps {
            echo 'I want to deploy the code'
          }
        }

      }
    }

  }
}