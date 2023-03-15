pipeline {
    agent any
        stages {
            stage('verifytools') {
                steps {
                    sh '''
                       export PATH=$PATH:/usr/local/bin
                       docker version
                       docker compose version
                       sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
                       sudo chmod +x /usr/local/bin/docker-compose
                       docker-compose version
                       curl --version
                       git --version
                   '''
             }
        }
    }
}
