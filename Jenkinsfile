pipeline {
  agent any
  stages {
    stage('compile') {
      stage ('Compile Stage') {
				steps {
					echo "Maven Compile"
					withMaven(maven : 'apache-maven-3.6.3') {
						bat 'mvn clean compile'
						
					}
				}
      }
    }

  }
}
