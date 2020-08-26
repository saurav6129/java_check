pipeline {
	agent none
	stages {
		stage('Java build') {
			agent {
				docker {
					image 'node:3.10.3'
				
				}
			}
		
			steps{
				sh'npm install'
				sh 'npm --version'
			
			}
		}
		
		
	}
}


