pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        sh '''docker build . -t django-app:latest












'''
        sh 'docker-compose up -d --no-deps --build web'
      }
    }

  }
  environment {
    djangopractice = ''
  }
}