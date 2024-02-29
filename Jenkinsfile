pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                bat 'npm install' 
            }
        }
		stage('Test') { 
            steps {
			
			    bat """
                   cd jenkins/scripts  
                   test.batch				  
                 """
			   
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