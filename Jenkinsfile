pipeline {
  agent {
    docker {
      image 'node'
    }
    
  }
  stages {
    stage('build') {
      agent {
        node {
          label 'node'
        }
        
      }
      steps {
        fileExists 'README.md'
      }
    }
    stage('Test') {
      steps {
        sh 'nvm --version'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Hello World'
      }
    }
  }
}