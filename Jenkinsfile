pipeline {
  agent any
  stages {
    stage('Pre') {
      steps {
        sh 'node -v'
        sh 'pnpm install'
      }
    }
    stage('Build') {
        steps {
            sh 'pnpm run build'
        }
    }
    stage('Test') {
        steps {
            echo 'Running test stage'
            echo 'Assuming tests are passed'
          }
      }
    stage('Deploy'){
        steps {
            echo 'Running deply stage'
            echo 'Assuming the code is deployed somewhere'
          }
      }
  }
  post {
      success {
          echo 'Hurray! We successfully ran jenkins pipeline'
          echo '@TODO create a simple script that will be going to send notification'
        }
      failure {
          echo 'Uh Oh! Test pipeline failed'
          echo '@TODO create a simple script that will be going to send notification'
        }
    }
}
