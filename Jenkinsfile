pipeline {
	agent any
	stages {

		stage('Build') {
			steps {
				sh 'cd lib/ ; wget https://repo1.maven.org/maven2/org/junit/platform/junit-platform-console-standalone/1.7.0/junit-platform-console-standalone-1.7.0-all.jar'
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
