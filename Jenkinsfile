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
			    bat """
                   cd jenkins/scripts  
				   deliver.batch
				 """
                  
            }
        }
    }
}