pipeline {
    agent {
        docker {
            image '8.16.1-jessie'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {	
                sh 'npm install'
            }
        }
    }
}
