pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'Testing Firefox1\''
          }
        }

        stage('Test Chrome') {
          steps {
            sh 'echo \'Testing Chrome1\''
          }
        }

        stage('Test Edge') {
          steps {
            sh 'echo \'Testing Edge1\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}