pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        echo 'code compilation'
        bat(script: 'javac -sourcepath src *.java', returnStdout: true, returnStatus: true)
      }
    }

  }
}