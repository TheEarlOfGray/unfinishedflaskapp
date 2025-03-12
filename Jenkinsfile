pipeline {
  agent any
  environment {
    SECRET_TEXT = credentials('SECRET_TEXT')
  }
  stages {
    stage('Build') {
      steps {
        sh 'pip install -r requirements.txt'
        sh 'python3 app.py'
      }
    }
  }
}
