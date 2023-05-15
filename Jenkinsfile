pipeline {
  agent any
  stages {
    stage('Checkout code') {
      steps {
        git(branch: 'main', url: 'https://github.com/suriya0304/docker-jenkins-ebs')
      }
    }

    stage('error') {
      parallel {
        stage('error') {
          steps {
            sh 'ls -la'
          }
        }

        stage('unit test') {
          steps {
            sh 'npm i && npm run test'
          }
        }

      }
    }

  }
}