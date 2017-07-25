pipeline {
#    agent { docker 'maven:3.3.3' }
agent {
    docker {
        image 'maven:3.3.3'
        label 'TEST-LABEL'
        args  '-v /tmp:/tmp'
    }
}
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
