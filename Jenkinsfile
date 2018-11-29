
pipeline {
  agent any
  stages {
    stage('install apache and start it') {
      steps {
        sh "yum update -y"
        sh "yum install httpd -y"
      }
    }
  }
}
