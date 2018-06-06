pipeline {
	agent none 
	stages {
		stage('Example Build') {
			agent { docker 'ubuntu:16.04' } 
			steps {
				echo 'Hello, Ubuntu'
				sh 'ls'
			}
		}
		stage('Example Test') {
			agent { docker 'openjdk:8-jre' } 
			steps {
				echo 'Hello, JDK'
				sh 'java -version'
			}
		}
	}
}