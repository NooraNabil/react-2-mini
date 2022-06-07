pipeline {
    agent any
    
    tools {nodejs "nodejs"}
    stages {
        stage('Git') {
      steps {
        git 'https://github.com/jellywiz/calculator.git/'
      }
    }
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Test'){
        	steps {
        		bat 'npm run test'
			}
		}
        stage('Deliver') {
            steps {
                bat 'npm start run'
            }
        }
    }
}
