pipeline {
  agent any
  stages {
    stage("verify tooling") {
      steps {
        sh '''
          /usr/local/bin/docker version
          /usr/local/bin/docker info
          /usr/local/bin/docker-compose version 
          /bin/curl --version
          /bin/jq --version
        '''
      }
    }
  }
}