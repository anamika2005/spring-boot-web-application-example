pipeline {
	agent any

	tools {
		maven 'Maven_Home'
		jdk 'JAVA8'
	
	}

	stages {
		stage('Init') {
			steps {
				sh '''
					echo "PATH = ${PATH}"
					echo "M2_HOME = ${M2_HOME}"
				'''
			}
		}

		stage ('Build') {
			steps {
				sh 'mvn install'
			}
		}
	}
}
