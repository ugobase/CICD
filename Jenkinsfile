pipeline {
  agent any
  stages {
    stage('Git') {
      steps {
        git(url: 'https://github.com/ugobase/CICD', branch: 'main')
      }
    }

    stage('Git Check') {
      steps {
        git(url: 'https://github.com/ugobase/CICD', branch: 'main')
      }
    }

  }
}