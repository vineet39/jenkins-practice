pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				echo "Build"
				echo "Something"
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
