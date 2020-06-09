pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        echo 'code compilation'
        bat(script: 'mvn compile -X', returnStdout: true, returnStatus: true)
      }
    }

    stage('Build') {
      steps {
        echo 'Building'
        bat 'mvn install -X'
      }
    }

  }
}