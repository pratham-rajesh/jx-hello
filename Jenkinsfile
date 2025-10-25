pipeline {
  // Runs on your default Jenkins agent; Docker agent is fine too if you prefer
  agent any

  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello World"'
        sh '''
          echo "Multiline shell steps works too"
          ls -lah
        '''
      }
    }
  }
}

