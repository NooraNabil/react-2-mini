pipeline {
    agent any
    
    tools {nodejs "nodejs"}
    stages {
        stage('Git') {
      steps {
        git 'https://github.com/NooraNabil/react-2-mini.git/'
      }
    }
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test'){
        	steps {
        		sh 'npm run test'
			}
		}
        stage('Deliver') {
            steps {
                sh 'npm start run'
            }
        }
    }
}
