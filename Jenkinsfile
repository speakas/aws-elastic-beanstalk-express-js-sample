pipeline {
    agent {
        // Using the Node 16 Docker image as the build agent
        docker {
            image 'node:16'
        }
    }
    stages {
        stage('Build') {
            steps {
                // Running npm install --save as a build step
                checkout scm
                sh 'npm install --save'
            }
        }
    }
}

