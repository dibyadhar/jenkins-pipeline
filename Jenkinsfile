pipeline {
  agent any
  stages {
    stage('Buzz Buzz') {
      steps {
        echo 'Bees Buzz!'
      }
    }

    stage('Bees Bees') {
      steps {
        echo 'Buzz, Bees, Buzz!'
      }
    }

    stage('Buzz test') {
      parallel {
        stage('Testing A') {
          steps {
            bat 'echo I am a %BUZZ_NAME%'
          }
        }

        stage('Testing B') {
          steps {
            bat 'timeout 10 '
            echo 'Done'
          }
        }

      }
    }

  }
  environment {
    BUZZ_NAME = 'Worker Bee'
  }
}