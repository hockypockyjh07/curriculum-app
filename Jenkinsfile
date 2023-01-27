pipeline {
  agent any
  stages {
    stage('Check out code') {
      steps {
        git(branch: 'dev', url: 'https://github.com/hockypockyjh07/curriculum-app')
      }
    }

    stage('Log directory') {
      parallel {
        stage('Log directory') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Frontend unit test ') {
          steps {
            sh 'cd curriculum-front && npm i && npm rum test:unit'
          }
        }

      }
    }

  }
}