pipeline {
    agent any
    stages { 
        stage('Test') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Build'){
            build job: 'HelloWorld'
        }
        stage('NodeTest'){
            node('linux_test'){
                sh 'hostname'
            }
        }
       stage('install'){
           steps{     
           sh 'mvn -install'
           }
       }
    }
}
