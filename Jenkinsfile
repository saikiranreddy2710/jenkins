pipeline {
    agent any
    environment {
        PATH = "/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/Applications/Docker.app/Contents/Resources/bin/:/Users/saikiranreddy/Library/Group\\ Containers/group.com.docker/Applications/Docker.app/Contents/Resources/bin"
    }
        stages {
            stage('verifytools') {
                steps {
                    sh '''
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
