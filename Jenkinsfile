pipeline {
	agent any

	stages {
		stage('Build') {
			steps {
				echo 'Building...'
				bat "mvn clean compile"
				archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
			}
		}
	
		stage('Test') {
			steps {
				echo 'Testing...'
			}
		}

		stage('Deploy') {
			steps {
				echo 'Deploying...'
			}
		}
	}
}