pipeline {
    agent any  // Rulează pe orice agent disponibil

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'make build'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'make test'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                sh 'make deploy'
            }
        }
    }
}
