pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        sh '''docker build . -t django-app:latest












'''
      }
    }

    stage('testing') {
      steps {
        sh 'docker-compose up -d --no-deps --build web'
      }
    }

  }
  environment {
    djangopractice = ''
  }
}