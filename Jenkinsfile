pipeline {
		agent any
		tools {
			maven 'maven'
		}
	stages {
		stage('init') {
			steps {
				echo 'Hola mundo'
			}
		}
		stage('build') {
			steps {
				sh 'mvn package'
			}
		}
		stage('finish') {
			steps {
				echo 'Done'
			}
		}
	}
}