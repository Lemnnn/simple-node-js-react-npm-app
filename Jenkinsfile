pipeline {
    agent {
        docker {
            image 'node:20-alpine'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
    }
    stages {
        stage('Test') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
    }
}