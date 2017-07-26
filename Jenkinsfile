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
    	stage ('JUNIT')
        always {
            junit 'build/reports/**/*.xml'
        }
    }
}
