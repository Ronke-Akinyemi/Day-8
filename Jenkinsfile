pipeline {
    agent { docker { image 'node:20.9.0-alpine3.18' } }
    stages {
        stage('build') {
            steps {
                script {
                    // Replace the following line with your local command
                    sh 'npm install'
                }
            }
        }
    }
}
