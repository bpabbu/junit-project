pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        readMavenPom(file: 'pom.xml')
      }
    }

  }
}