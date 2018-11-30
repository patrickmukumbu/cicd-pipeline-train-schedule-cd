
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        stage('Test') {
            when {
                branch 'master'
            }
            steps {
                sh 'ls / >> /tmp/test.txt'
                }
            }
        stage('kuangalia'){
            steps {
                echo 'Checking kama kila kitu iko sawa'
            }
        }
        
        }
       
    
}
