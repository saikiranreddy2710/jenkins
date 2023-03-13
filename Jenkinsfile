pipeline {
    agent any
        stages {
            stage('verifytools') {
                steps {
                    sh '''
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
