pipeline {
  agent any
  environment {
    SECRET_TEXT=credentials('SECRET_TEXT')
  }
  stages {
    stage('Build') {
      steps {
        sh 'sudo echo $SECRET_TEXT > /home/ubuntu/secret.txt'
        sh 'pip install -r requirements.txt'
        sh 'python3 app.py'
      }
    }
  }
}
