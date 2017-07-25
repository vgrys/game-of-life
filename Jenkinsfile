pipeline {
    agent any
	tools {
	maven 'maven:3.3.3' 
	}
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
	  }
        }
    }
}
