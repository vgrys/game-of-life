pipeline {
    agent any
	tools {
	maven 'Default' 
	}
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
	  }
        }
    }
}
