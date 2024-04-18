pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh '''
                PATH=/sbin:/bin:/usr/sbin:/usr/bin:/usr/syno/sbin:/usr/syno/bin:/usr/local/sbin:/usr/local/bin
                export PATH
                echo $PATH
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