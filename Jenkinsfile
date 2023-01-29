pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''npm ci


'''
      }
    }

    stage('Test') {
      steps {
        sh '''npm test
'''
      }
    }

    stage('Pack') {
      steps {
        sh '''npm build
ls -ltr
'''
      }
    }

  }
}