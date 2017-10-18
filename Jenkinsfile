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
       stage('node') {
            parallel Slave: {
                node('linux_test') {
                    echo "in slave server"
                }
             },
            Master: {
                node('master') {
                    echo "in master server"
                }
        }
    }
}
