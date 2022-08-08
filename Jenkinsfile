pipeline {
    agent {
        docker {
            image 'node:lts-slim'
            args '-p 3000:3000 -p 5000:5000 -u root'
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
    }
}
