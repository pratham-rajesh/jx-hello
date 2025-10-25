pipeline {
  agent {
    // Spin up a fresh container for this run
    docker { image 'node:22-alpine' }
  }

  stages {
    stage('Test') {
      steps {
        // Show what environment we're actually in
        sh 'node --eval "console.log(process.arch, process.platform)"'
        // A couple of extra sanity checks (feel free to keep them)
        sh 'which node && node -v'
        sh 'uname -a'
      }
    }
  }
}

