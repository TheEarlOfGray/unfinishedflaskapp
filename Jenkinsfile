pipeline {
  agent any
  environment {
    SECRET_TEXT=credentials('SECRET_TEXT')
  }
  stages {
    stage('Build') {
      steps {
        sh 'echo $SECRET_TEXT'
        sh 'pip install -r requirements.txt'
        sh 'python3 app.py'
      }
    }
  }
}
