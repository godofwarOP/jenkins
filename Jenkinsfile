pipeline {
  agent any
  stages {
    stage('Pre') {
      steps {
        sh 'node -v'
        sh 'npm install -g pnpm'
        sh 'pnpm install'
      }
    }
  }
}
