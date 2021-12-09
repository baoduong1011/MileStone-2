pipeline {
	agent any
	stages {

		stage('Build') {
			steps {
				sh 'cd lib/'
			}
		}

		stage('Test') {
			steps {
				echo "Test Jenkins"
			}
		}

		stage('Deploy') {
			steps {
				echo "Deploy Jenkins"
			}
		}
	}
}
