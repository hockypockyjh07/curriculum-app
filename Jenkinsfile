pipeline {
  agent any
  stages {
    stage('Check out code') {
      steps {
        git(branch: 'dev', url: 'https://github.com/hockypockyjh07/curriculum-app')
      }
    }

    stage('Log directory') {
      steps {
        sh 'ls -la'
      }
    }

    stage('Build') {
      steps {
        sh 'docker build -f curriculum-front/Dockerfile .'
      }
    }

  }
}