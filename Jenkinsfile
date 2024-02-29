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
			    cd  'jenkins\scripts'
                start 'test.batch' 
            }
        }
    }
}