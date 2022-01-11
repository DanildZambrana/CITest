pipeline {
    
    agent any
    
    stages {
        stage('openjdk:7-jdk') {
            agent {
                docker {
                    image 'jdk7_image'
                }
            }
            
            steps {
                
                sh 'java -version'
            }
        }
        
        stage('java8') {
            agent {
                docker {
                    image 'openjdk:8-jdk'
                }
            }
            
            steps {
                sh 'java -version'
            }
        }
    }
}
