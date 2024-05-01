pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'i will prit'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'build it'
          }
        }

        stage('test') {
          steps {
            echo 'i will test'
          }
        }

        stage('deploy') {
          steps {
            echo 'i will deploy'
          }
        }

      }
    }

  }
}