pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        echo 'Build It'
        waitUntil()
      }
    }
    stage('Deploy') {
      steps {
        sleep 30
      }
    }
  }
}