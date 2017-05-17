pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'php build.php' 
            }
        }
	    

	stage('Login and Browse'){
            steps {
                sh 'php frontend1.php'
            }
		}


	 stage('Contacts '){
            steps {
                sh 'php frontend2.php'
            }
                }
	    
	 stage('Api tests'){
            steps {
                sh 'php backend.php'
            }
	 }
	    
	    
        stage('Deploy') {
            steps {
                sh 'php deploy.php'
            }
        }
    }
