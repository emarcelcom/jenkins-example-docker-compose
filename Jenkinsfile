pipeline {
  agent any
  stages {
    stage("verify tooling") {
      steps {
        sh '''
          PATH=/sbin:/bin:/usr/sbin:/usr/bin:/usr/syno/sbin:/usr/syno/bin:/usr/local/sbin:/usr/local/bin
          export PATH
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