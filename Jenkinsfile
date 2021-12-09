pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				sh 'mkdir lib'
				sh 'cd lib/ wget https://repo1.maven.org/maven2/org/junit/platform/junit-platform-console-standalone/1.7.0/junit-platform-console-standalone-1.7.0-all.jar'
				sh 'cd src; javac -cp "../lib/junit-platform-console-standalone-1.7.0-all.jar" /main/java/launch/Main.java'
			}
		}
		stage('Test') {
			steps {
				sh 'cd src/ ; java -jar ../lib/junit-platform-console-standalone-1.7.0-all.jar -cp "." --select-class Main --reports-dir="reports"'
			}
		}
		stage('Deploy') {
			steps {
				sh 'mvn clean install'
			}
		}
	}
}
