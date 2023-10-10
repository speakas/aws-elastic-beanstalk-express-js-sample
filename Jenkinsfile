pipeline {
    agent any
    stages {
        stage('Debug Docker') {
            steps {
                script {
                    echo "DOCKER INFO:"
                    sh "docker info || true"
                    echo "ENV VARIABLES:"
                    sh "env || true"
                }
            }
        }
        stage('Build') {
            agent {
                docker {
                    image 'node:16'
                }
            }
            steps {
                sh 'npm install --save'
            }
        }
    }
}
