@Library("Shared") _
pipeline {
  agent {
    docker { image 'node:16-alpine' }
  }
  stages {
    stage('Hello') {
      steps {
        script{
          hello()
        }
      }
    }
    stage('Test') {
      steps {
        sh 'node --version'
      }
    }
  }
}
