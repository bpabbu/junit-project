pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        readMavenPom(file: 'pom.xml')
      }
    }

    stage('compile') {
      steps {
        bat 'mvn compile -X'
      }
    }

  }
}