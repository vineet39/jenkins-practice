pipeline {
	agent any
	environment {
		dockerHome = tool 'myDocker'
		mavenHome = tool 'myMaven'
		PATH = '$dockerHome/bin:$mavenHome:build:$PATH'
	}
	stages {
		stage('Build') {
			steps {
				echo "Build"
				echo "Somethingg"
				sh 'maven --version'
				sh 'docker version'
			}
		}
		stage('Test') {
			steps {
				echo "Test"
				echo "Something"
			}
		}
		
	}
	post {
			success {
				echo "Build successful"
			}
			failure {
				echo "Build failed"
			}
		}
}
