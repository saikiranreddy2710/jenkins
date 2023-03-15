pipeline {
    agent any
        stages {
            stage('verifytools') {
                steps {
                    sh '''
                       export PATH=$PATH:/usr/local/bin
                       docker version
                       docker compose version
                       curl --version
                       git --version
                   '''
             }
        }
    }
}
