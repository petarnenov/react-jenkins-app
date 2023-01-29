pipeline {
    agent {label 'docker-agent-alpine'}
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'ls -ltr'
                //sh 'docker build -t react-app .'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying..'
                // sh 'docker run --rm -d -p 80:80 react-app:latest'
            }
        }
    }
}