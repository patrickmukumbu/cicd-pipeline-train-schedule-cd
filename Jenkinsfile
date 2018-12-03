pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    ls / >> /tmp/example.txt
                    yum update -y
                '''
            }
        }
    }
}
