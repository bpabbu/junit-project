pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        echo 'code compilation'
        bat(script: 'javac -sourcepath src', returnStdout: true, returnStatus: true)
      }
    }

  }
}