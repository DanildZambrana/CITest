pipeline {
    
    agent any
    
    stages {
        stage('openjdk:7-jdk') {
            tools {
                jdk 'jdk-11;
            }
            steps {
                sh 'java -version'
            }
        }
    }
}
