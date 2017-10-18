pipeline {
    agent any
    stages { 
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
       stage('compile'){
           steps{     
           sh 'maven -version'
           }
       }
    }
}
