pipeline {
	agent any
	stages {
		stage('Build first') {
					steps {
						sh 'sleep 15; echo "This is a Build stage"'
					}
				}
				
				stage('Test'){
					steps {
						sh '''
							sleep 15
							echo "This is a Test stage"
						'''	
						git branch: 'main', url: 'https://github.com/jaintpharsha/devops-jan-22.git'
					}
				}
			} 
		}
		stage('Deploy'){
			steps {
				sh '''
					sleep 5
					echo "This is a Deploy stage"
				'''
			}
		}
		
		stage('am checking'){
			steps {
				sh '''
					sleep 5
					echo "This is a My-stage stage"
				'''
			}
		}	
}
