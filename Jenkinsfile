pipeline {
  agent { docker { image 'node:22-alpine' } }

  stages {
    stage('Test') {
      steps {
        sh 'echo "DOCKER: $(which docker || echo not-found)"'
        sh 'node --eval "console.log(process.arch, process.platform)"'
        sh 'node -v'
      }
    }
  }
}

