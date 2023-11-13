pipeline {
    agent any

    stages {
        stage('Install Docker') {
            steps {
                script {
                    // Install Docker on the Jenkins agent
                    sh 'curl -fsSL https://get.docker.com/ | sh'
                    sh 'sudo usermod -aG docker $USER'  // Add the current user to the docker group
                    sh 'newgrp docker'  // Activate the changes to the user's group membership
                }
            }
        }

        stage('Build') {
            agent { docker { image 'node:20.9.0-alpine3.18' } }
            steps {
                script {
                    // Replace the following line with your local command
                    sh 'npm install'
                }
            }
        }
    }
}
