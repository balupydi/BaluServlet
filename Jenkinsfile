pipeline{
	agent any
	
	node('master'){
		checkout scm
		stages{
			stage('compile'){
				steps{
					sh 'mvn clean install'
				}
			}
		}
	}
}
