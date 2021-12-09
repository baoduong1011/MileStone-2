pipeline {
	agent any
	stages {

		stage('Build') {
			steps {
				echo '==== WGET MAVEN ===='
				sh "cd lib/; /usr/local/bin/wget  https://repo1.maven.org/maven2/org/junit/platform/junit-platform-console-standalone/1.8.2/junit-platform-console-standalone-1.8.2-javadoc.jar"
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
