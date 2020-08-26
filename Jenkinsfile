pipeline {
	agent none
	stages {
		stage('Java build') {
			agent {
				docker{
					image 'node:6.3'
				}
			}
		}
		
		steps{
			sh'npm install'
			sh 'npm --version'
			
		}
		
	}
}