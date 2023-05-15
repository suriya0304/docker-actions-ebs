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
            sh 'pwd'
          }
        }

        stage('unit test') {
          steps {
            sh 'npm i && npm run test'
          }
        }

      }
    }

    stage('build') {
      steps {
        sh 'docker build -f Dockerfile .'
      }
    }

  }
}