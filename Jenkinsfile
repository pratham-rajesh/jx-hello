pipeline {
  agent { docker { image 'python:3.12-alpine' } }
  stages {
    stage('build') {
      steps {
        sh 'python --version'
      }
    }
  }
}
