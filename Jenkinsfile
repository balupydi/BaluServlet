pipeline {
    agent any
    stages { 
        stage('Test') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Build'){
            steps{
                build job: 'HelloWorld'
            }
        }
       stage('install'){
           steps{     
           sh 'mvn install'
           }
       }
    }
}
