pipeline {
    agent any
	tools {
	maven 'Default' 
	}
    stages {
         stage('Build') {
      		// Run the maven build
      		if (isUnix()) {
       	 	sh "'${mvnHome}/bin/mvn' -Dmaven.test.failure.ignore -Dmaven.test.skip.exec=true clean package"
     	 	} else {
         	bat(/"${mvnHome}\bin\mvn" -Dmaven.test.failure.ignore clean package/)
      		}
    		}
	stage ('testing') {
       		sh "'${mvnHome}/bin/mvn' -Dmaven.test.failure.ignore -Dtest='JmsDurable*' test"
   		}
   	stage('Results') {
		junit '**/target/surefire-reports/TEST-*.xml'
      		archive 'target/*.jar'
   	}
    }
}
