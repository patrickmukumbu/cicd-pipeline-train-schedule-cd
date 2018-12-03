pipeline {
    agent none
    stages {
        stage('Test on staging') {
            agent { 
                label 'staging'
            }
            steps {
                sh """
                    ls / >> /tmp/staging.txt
                    yum update -y
                """
            }
            
        }
        stage('Test on production') {
            agent {
                label 'production'
            }
            steps {
               sh """
                    ls / >> /tmp/production.txt
                    yum update -y
                """  
            }
            
        }
    }
}
