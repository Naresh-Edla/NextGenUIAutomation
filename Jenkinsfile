pipeline {
  agent {
    node {
      label 'master'
    }
    
  }
  stages {
    stage('build') {
      steps {
        sh 'echo "Setup python virtual environment"'
        sh 'echo "Install Code analyser and Unit test framework"'
        sh 'echo "Install all required packages"'
      }
    }
    stage('Test') {
      parallel {
        stage('Code Analyer') {
          steps {
            sh 'echo "Code Analyser"'
          }
        }
        stage('Unit Test') {
          steps {
            sh 'echo "Unit Test Done"'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "Deploy to environment"'
      }
    }
  }
}