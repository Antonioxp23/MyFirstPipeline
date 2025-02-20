pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building project...'
                sh 'make build'  // Rulează comanda de build
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'make test'  // Rulează testele
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'make deploy'  // Deploy automat
            }
        }
    }
}
