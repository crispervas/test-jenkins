pipeline {
  agent any
  tools {
    nodejs 'NODEJS'
  }

  options {
    timeout(time: 2, unit: 'MINUTES')
  }

  stages {
    stage('Install dependencies') {
      steps {
        sh 'ls && npm i'
      }
    }
    stage('Run tests') {
      steps {
        sh 'ls && npm t'
      }
    }
  }
}