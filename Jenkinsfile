pipeline {
    agent any
    environment {
        DOCKER_CRED = "docker-registry-deploy_srv-credentials-id"
        DOCKER_IMAGE = "itf"
    }
    stages {
        stage('Deploy test') {
            steps {
                script {
                     sshagent(credentials : ['ubuntu-antony']) {
                         sh "echo pwd"
                         sh 'ssh -t -t antony@192.168.0.199 -o StrictHostKeyChecking=no "echo pwd && ls -la"'
                    }
                }
            }
        }
    }
}
