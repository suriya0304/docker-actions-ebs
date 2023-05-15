pipeline {
  agent any
  stages {
    stage('Checkout code') {
      steps {
        git(branch: 'main', url: 'https://github.com/suriya0304/docker-jenkins-ebs')
      }
    }

    stage('') {
      steps {
        sh 'ls -la'
      }
    }

  }
}