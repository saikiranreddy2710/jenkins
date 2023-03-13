pipeline {
    agent any {
        stages {
            stage('verifytools'){
                sh ''' 
                   docker info
                   docker version
                   docker compose version
                   docker-compose version
                   curl --version
                   git --version
                   '''
            }
        }
    }
}