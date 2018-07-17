pipeline {
	agent any

	stages {
		stage('Startup') {
			steps {
				echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
			}
		}
		stage('Build') {
			steps {
				echo 'Building...'
				bat "mvn clean compile"
			}
		}
	
		stage('Test') {
			steps {
				echo 'Testing...'
				bat "mvn test"
			}
		}

		stage('Deploy') {
			steps {
				echo 'Deploying...'
			}
		}
	}
}