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
                sh 'pwd'
                sh 'hostname'
                sh 'whoami'
            }
        }
        stage('Build') {
            steps {
                sh 'sudo npm install' 
            }
        }
    }
}
