pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh '''
                . .bashrc
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