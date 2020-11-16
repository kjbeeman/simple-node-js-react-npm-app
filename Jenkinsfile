pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Debug') { 
            steps {
                sh 'ls'
            }
        }
        stage('Build') {
            steps {
                sh 'npm install' 
            }
        }
    }
}
