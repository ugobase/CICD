pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/ugobase/CICD', branch: 'main')
      }
    }

    stage('Checking') {
      steps {
        sh 'ls -la'
      }
    }

    stage('Docker Login') {
      environment {
        DOCKERHUB_USER = 'ugobase'
        DOCKERHUB_PASSWORD = 'Nwaoluwa100%'
      }
      steps {
        sh 'docker login -u $DOCKERHUB_USER -p $DOCKERHUB_PASSWORD'
      }
    }

  }
}