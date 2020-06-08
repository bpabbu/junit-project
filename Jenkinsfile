pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        cleanWs(cleanWhenFailure: true)
        bat 'junit-project/pom.xml'
      }
    }

  }
}