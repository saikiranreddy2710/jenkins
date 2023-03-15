pipeline {
    agent any
        stages {
            stage('verifytools') {
                steps {
                    sh '''
                       export PATH=$PATH:/usr/local/bin
                       docker version
                       docker compose version
                       echo S@i@2710 | sudo -S curl -L https://github.com/docker/compose/releases/download/1.29.2/docker-compose-Darwin-arm64 -o /usr/local/bin/docker-compose
                       sudo chmod +x /usr/local/bin/docker-compose
                       docker-compose --version
                       curl --version
                       git --version
                   '''
             }
        }
    }
}
