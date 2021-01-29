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

    stage('Buzz Test') {
      steps {
        bat 'echo I am a ${BUZZ_NAME}'
      }
    }

  }
  environment {
    BUZZ_NAME = 'Worker Bee'
  }
}