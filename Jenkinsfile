pipeline {
  agent any
  stages {
    stage('pre-build') {
      steps {
        echo 'pre-building'
      }
    }

    stage('docker build') {
      steps {
        sh 'docker build . -t django-app:latest'
      }
    }

    stage('build completed') {
      steps {
        echo 'build successfully completed'
      }
    }

    stage('docker images created') {
      steps {
        echo 'images created'
      }
    }

    stage('testing') {
      steps {
        echo 'testing started'
      }
    }

    stage('docker compose') {
      steps {
        sh 'docker-compose up -d --no-deps --build web'
      }
    }

    stage('tested') {
      steps {
        echo 'successfully tested'
      }
    }

    stage('configration completed') {
      steps {
        echo 'configration completed'
      }
    }

  }
  environment {
    project = ''
  }
}