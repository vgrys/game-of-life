pipeline {
<<<<<<< HEAD
agent {
    docker {
        image 'maven:3.3.3'
        args  '-v /tmp:/tmp'
    }
}
=======
    agent { 'maven:3.3.3' }
>>>>>>> master
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
