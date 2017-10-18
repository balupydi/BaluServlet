pipeline{
	agent any
	node('master'){
		stages{
			stage('compile'){
				steps{
					sh 'mvn clean install'
				}
			}
		}
	}
}
