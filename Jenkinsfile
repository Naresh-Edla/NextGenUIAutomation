pipeline {
  agent {
    node {
      label 'master'
    }
    
  }
  stages {
    stage('build') {
      steps {
        sh 'ls'
      }
    }
    stage('Test') {
      steps {
        sh 'echo "Code Analyser"'
        sh 'echo "Unit Test"'
      }
    }
  }
}