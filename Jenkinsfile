pipeline {
    agent any

    stages {       
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