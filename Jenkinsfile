pipeline {
  agent any
  stages {
    stage("verify tooling") {
      steps {
        sh '''
          #!/bin/bash
          set -x  # Print executed commands for debugging
          export PATH=$PATH:/usr/local/bin  # Add Docker path if needed
          docker version
          docker info
          docker-compose version 
          curl --version
          jq --version
        '''
      }
    }
  }
}