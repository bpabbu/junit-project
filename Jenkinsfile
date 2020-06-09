pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        echo 'code compilation'
        bat(script: 'javac *.java', returnStdout: true, returnStatus: true)
      }
    }

  }
}