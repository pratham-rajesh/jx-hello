pipeline {
  agent { docker { image 'node:22-alpine' } }

  environment {
    // Append /usr/local/bin in front of whatever PATH Jenkins already has
    PATH = "/usr/local/bin:${env.PATH}"
  }

  stages {
    stage('Test') {
      steps {
        // Sanity checks
        sh 'echo "DOCKER: $(which docker || echo not-found)"'
        sh 'node --eval "console.log(process.arch, process.platform)"'
        sh 'node -v'
      }
    }
  }
}
