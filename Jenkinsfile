pipeline {
    agent any
    environment {
        CI = 'true'  // Corrected the typo
    }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'  // Added space after bat for readability
            }
        }
        stage('Test') {
            steps {
                bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "chmod +x ./jenkins/scripts/test.sh && ./jenkins/scripts/test.sh"'
            }
        }
    }
}
