pipeline {
  agent any
  stages {
    stage('Pre') {
      steps {
        sh 'node -v'
        sh 'sudo npm install -g pnpm'
        sh 'pnpm install'
      }
    }
  }
}
