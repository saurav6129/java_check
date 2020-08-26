pipeline {
	agent none
	stages {
		stage('Java build') {
			agent {
				docker {
					image 'node:6.3'
				
				}
			}
		
			steps{
				sh 'npm --version'
			
			}
		}
		
		stage(' Maven Build') {
			agent {
				docker {
					image 'maven:3-alpine'
					args '-v /root/.m2:/root/.m2'
				}
			}
			
            steps {
				sh 'mvn test'
				
            }
			
        }
	}
}


