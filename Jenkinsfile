pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        echo 'code compilation'
        bat(script: 'mvn compile', returnStdout: true, returnStatus: true, encoding: 'javac')
      }
    }

  }
}