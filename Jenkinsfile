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

    stage('Unit test') {
      steps {
        sh './mvnw test'
        junit '**/target/surefire-reports/TEST-*.xml'
      }
    }

  }
}