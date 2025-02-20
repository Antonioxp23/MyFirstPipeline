pipeline {
    agent any
    environment {
        GIT_CREDENTIALS_ID = 'github-token'  // ID-ul credențialei salvate
    }
    stages {
        stage('Checkout') {
            steps {
                withCredentials([usernamePassword(credentialsId: GIT_CREDENTIALS_ID, usernameVariable: 'GIT_USER', passwordVariable: 'GIT_PASS')]) {
                    sh 'git clone https://$GIT_USER:$GIT_PASS@github.com/user/repository.git'
                }
            }
        }
    }
}
