pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build...'
      }
    }

    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'Testing firefox\''
          }
        }

        stage('Test Chrome') {
          steps {
            sh 'echo \'Test Chrome\''
          }
        }

        stage('Test Edge') {
          steps {
            sh 'echo \'Testin Edge\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy...'
      }
    }

  }
}