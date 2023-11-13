pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Add your macOS-specific commands here
                    sh 'docker --version'  // Check Docker version
                    sh 'npm install'  // Your actual build steps using Docker
                }
            }
        }
    }
}

