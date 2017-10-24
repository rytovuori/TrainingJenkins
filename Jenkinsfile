pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'nvm --version'
      }
    }
    stage('Test') {
      steps {
        fileExists 'README.md'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Hello World'
      }
    }
  }
}