pipeline {
    agent any

    stages {
        stage('Ohne Docker') {
            steps {
                sh 'echo "Hello World, ohne Docker"'
            }
        }
        
        stage('Mit Docker') {
            agent {
                docker {
                    image 'node:18-alpine'
                }
            }
            
            steps {
                sh 'echo "Hello World, mit Docker"'
                sh 'npm --version'
            }
        }
    }
}