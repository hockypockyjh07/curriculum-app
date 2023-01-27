pipeline {
  agent any
  stages {
    stage('Check out code') {
      steps {
        git(branch: 'dev', url: 'https://github.com/hockypockyjh07/curriculum-app')
      }
    }

    stage('Directory') {
      steps {
        sh 'ls -la'
      }
    }

  }
}