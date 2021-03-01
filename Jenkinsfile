pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo \'Building ...\''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh 'echo \'Testing Chrome...\''
          }
        }

        stage('Testing Firefox') {
          steps {
            sh 'echo \'Testing Firefox...\''
          }
        }

        stage('Testing Edge') {
          steps {
            sh 'echo \'Testing Edge...\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sh 'echo \'Deploying\''
      }
    }

  }
}