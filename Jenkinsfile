pipeline {
    agent any
	tools {
	maven 'maven:Default' 
	}
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
	  }
        }
    }
}
