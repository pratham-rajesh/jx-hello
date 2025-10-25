pipeline {
  agent { docker { image 'node:22-alpine' } }
  environment {
    "PATH+EXTRA" = "/usr/local/bin"
  }
  stages {
    stage('Test') {
      steps {
        sh 'echo DOCKER=$(which docker || echo "not-found")'
        sh 'node --eval "console.log(process.arch, process.platform)"'
        sh 'node -v'
      }
    }
  }
}

