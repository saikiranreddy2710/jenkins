pipeline {
    agent any
        stages {
            stage('verifytools') {
                steps {
                    sh '''
                       export PATH=$PATH:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/Applications/Docker.app/Contents/Resources/bin/:/Users/XXX/Library/Group\ Containers/group.com.docker/Applications/Docker.app/Contents/Resources/bin
                       docker version
                       docker compose version
                       docker-compose --version
                       curl --version
                       git --version
                   '''
             }
        }
    }
}
