pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'I want to build'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'I Want to test'
          }
        }

        stage('Deploy') {
          steps {
            echo 'I want to deploy'
          }
        }

      }
    }

  }
}