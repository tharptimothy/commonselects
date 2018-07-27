pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        echo 'Build It'
        waitUntil() {
          input 'Depoly'
        }

      }
    }
    stage('Deploy') {
      steps {
        sleep 30
      }
    }
  }
}