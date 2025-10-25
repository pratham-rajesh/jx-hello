pipeline {
  agent { docker { image 'python:3.12-alpine' } }
  stages {
    stage('build and inspect') {
      steps {
        sh 'python --version'
        sh 'echo "Hello from Jenkins pipeline"'
        sh '''
           echo "Listing workspace contents"
           ls -lah
        '''
      }
    }
  }
}
