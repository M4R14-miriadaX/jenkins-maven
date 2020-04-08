pipeline {
		agent any
		tools {
			maven 'maven'
		}
	stages {
		stage('Inicio') {
			steps {
				echo 'Iniciando construcción automática'
			}
		}
		stage('Testeo') {
			steps {
				echo 'Ejecutando pruebas del proyecto'
				bat 'mvn test'
			}
		}
		stage('Empaquetado') {
			steps {
				echo 'Empaquetando la aplicación'
				bat 'mvn package'
			}
		}
		stage('Ejecución') {
			steps {
				bat 'mvn exec:java -Dexec.mainClass="com.maria.app.Practica2.App"'
			}
		}
		stage('Fin') {
			steps {
				echo 'El proyecto se ha construido'
			}
		}
	}
}