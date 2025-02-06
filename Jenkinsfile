pipeline {
    agent any

    stages {
        stage('Hello mit Docker') {
            agent {
                docker {
                    image 'node:18-alpine'
                    reuseNode true
                }
            }

            steps {
                sh '''
                echo 'Hello World, mit Docker'
                touch exe-container.txt
                node --version
                npm --version
                '''
            }
        }
    }
}