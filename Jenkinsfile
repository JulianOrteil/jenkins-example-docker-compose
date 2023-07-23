pipeline {
    agent any
    stages {
        stage("verify tooling") {
            steps {
                ssh '''
                    docker info
                    docker version
                    docker compose version
                    curl --version
                    jq --version
                '''
            }
        }
    }
}