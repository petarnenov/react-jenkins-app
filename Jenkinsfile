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
        sh '''npm run build
ls -ltr
'''
      }
    }

    stage('Deploy') {
      steps {
        sh '''docker cp build/ c265c76248d2:/usr/share/nginx/html

'''
      }
    }

  }
}