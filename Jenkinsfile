pipeline {
    agent any
    environment {
        DOCKER_CRED = "docker-registry-deploy_srv-credentials-id"
        ENVIRONMENT = getEnvironment()
        DOCKER_IMAGE = "itf"
    }
    stages {
        stage('Deploy test') {
            steps {
                script {
                    ls -la
                }
            }
        }
    }
}
