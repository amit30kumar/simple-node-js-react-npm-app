pipeline {
    agent none
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example Test') {
            agent { docker 'maven:3-eclipse-temurin-11' }  
            steps {
                echo 'Hello, Maven'
                sh 'mvn --version'
            }
        }
    }
}
