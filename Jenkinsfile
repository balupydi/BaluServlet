pipeline {
    agent any
    stages { 
        stage('Example') {
            steps {
                echo 'Hello World'
            }
            stage('compile'){
                sh 'maven -version'
            }
        }
    }
}
