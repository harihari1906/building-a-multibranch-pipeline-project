pipeline {
    agent any
    envivironment{
        CI ='true'
    }
    stages {
        stage('Build') {
            steps {
                bat'npm install'
            }
        }
        stage('test'){
            steps{
                bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "chmod +x ./jenkins/scripts/test.sh && ./jenkins/scripts/test.sh"'
            }
        }
    }
}
