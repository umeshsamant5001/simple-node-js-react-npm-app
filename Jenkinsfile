pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                bat 'npm install' 
            }
        }
		stage('Deliver') {
            steps {
			    bat 'npm run build'
				bat 'npm start'
                  
            }
        }
    }
}