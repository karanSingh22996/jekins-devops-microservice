//SCRIPTED

//DECLARTIVE
pipeline {
	//agent any
	agent {docker {image 'maven'}}
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
				echo "Build"
			}
		}
		stage('Test'){
			steps {
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	}
	post {
		always {
			echo "I am awesome and I always run"
		}
		success {
			echo "I run when pipeline success"
		}
		failure {
			echo "I run when pipeline fails"
		}
	}
}