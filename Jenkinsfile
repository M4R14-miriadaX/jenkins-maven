pipeline {
		agent any
		tools {
			maven 'maven'
		}
	stages {
		stage('Inicio') {
			steps {
				echo 'Iniciando...'
			}
		}
		stage('Testeo') {
			steps {
				bat 'mvn test'
			}
		}
		stage('Empaquetado') {
			steps {
				bat 'mvn package'
			}
		}
		stage('Fin') {
			steps {
				echo 'Build terminado.'
			}
		}
		stage('Ejecución') {
			steps {
				bat 'mvn exec:java -Dexec.mainClass="com.maria.app.App"'
			}
		}
	}
}