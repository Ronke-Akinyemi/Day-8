pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Replace '/usr/local/bin/docker' with the actual full path
                    sh '/usr/local/bin/docker --version'
                }
            }
        }
    }
}
