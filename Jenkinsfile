pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh 'docker build -t todo .'
        sh 'docker run -d -p 8000:8000 todo'
      }
    }
  }
}
