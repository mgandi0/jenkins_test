pipeline {
    agent any
    
    environment {
        TRAINING = "devops"
        TOPIC = "jenkins"
    }
    
    stages {
        stage('local') {
            environment {
                TOPIC = "cicd"
            }
            
            steps {
                sh "echo training is ${TRAINING} and topic is ${TOPIC}"
            }
        }
        
        stage('global') {
            steps {
                sh "echo training is ${TRAINING} and topic is ${TOPIC}"
            }
        }
    }
}
