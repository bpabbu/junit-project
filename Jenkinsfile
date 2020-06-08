pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        readMavenPom(file: 'pom.xml')
      }
    }

    stage('compile') {
      agent any
      steps {
        bat 'mvn compile -Dmaven.main.skip'
      }
    }

  }
}