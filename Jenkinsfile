pipeline {
	agent any
		tools {
        maven "apache-maven-3.6.3"
        jdk "jdk-14.0.1"
		}
		stages {
			stage ('Compile Stage') {
				steps {
					echo "Maven Compile"
					withMaven(maven : 'apache-maven-3.6.3') {
						bat 'mvn clean compile'
						
					}
				}
			}
			stage ('Testing Stage') {
				steps {
					echo "Testing Stage"
					withMaven(maven : 'apache-maven-3.6.3') {
						bat 'mvn test'
					}
				}
			}
			stage ('Deployment Stage') {
				steps {
					echo "Deployment Stage"
					withMaven(maven : 'apache-maven-3.6.3') {
						bat 'mvn deploy -X'
					}
				}
			}
			stage ('Install Stage') {
				steps {
					echo "Install Stage"
					withMaven(maven : 'apache-maven-3.6.3') {
						bat 'mvn install -U -X'
					}
				}
			}
		}
	}
