pipeline {
    agent { node { label 'agent-1' } }

    stages {
        stage('install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Unit test') {
            steps {
                echo 'unit testing stage'
            }
        }
        stage('Sonar Scan') {
            steps {
                sh 'ls -ltr'
                sh 'sonar-scanner'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deplyment'
            }
        }
    }
}