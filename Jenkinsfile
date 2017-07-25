pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
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
