pipeline {
    
    agent any
    tools {
        jdk 'jdk-11'
    }
    
    stages {
        stage('build') {        
            steps {
                sh 'mvn compile -Dmaven.test.skip'
            }
        }
        
        stage('test') {
            steps {
                sh 'mvn test'
            }
        }
        
        stage('deploy') {
            steps {
                sh 'mvn clean package -Dmaven.test.skip'
            }
        }
    }
}
