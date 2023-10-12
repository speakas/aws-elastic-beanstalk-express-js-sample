pipeline {
    agent {
        docker {
            image 'node:16' // use Node 16 Docker image as the build agent
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install --save' // run npm install command
            }
        }
    }
}
