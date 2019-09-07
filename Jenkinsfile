pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    environment {
	CI = 'true'
    }
    stages {
        stage('Build') {
            steps {	
		npm config set registry http://registry.npmjs.org
                sh 'npm install'
            }
        }
    }
}
