
pipeline {
    agent 'staging'
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
                sh 'yum update -y'
                }
            }
        
        }
       
    }
}
