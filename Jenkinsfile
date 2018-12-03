pipeline {
    agent none
    stages {
        stage('Test on staging') {
            agent any
            steps {
                sh """
                    ls / >> /tmp/staging.txt
                    yum update -y
                """
            }
            
        }
        stage('Test on production') {
            agent any
            steps {
               sh """
                    ls / >> /tmp/production.txt
                    yum update -y
                """  
            }
            
        }
    }
}
