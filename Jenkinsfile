pipeline {
  agent {
    docker {
      image 'node'
    }
    
  }
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