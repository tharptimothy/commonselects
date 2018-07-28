pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        echo 'Build It'
        sshagent()
      }
    }
  }
}