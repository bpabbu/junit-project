pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        cleanWs(cleanWhenFailure: true)
        readMavenPom(file: 'pom.xml')
      }
    }

  }
}