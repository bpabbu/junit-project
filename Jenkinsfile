pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        cleanWs(cleanWhenFailure: true)
        bat 'mvn install -X'
      }
    }

  }
}