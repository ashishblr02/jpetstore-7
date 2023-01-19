pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Print message'
        sh '''./mvnw clean compile
'''
      }
    }

    stage('Test') {
      steps {
        sh './mvnw test'
      }
    }

  }
}