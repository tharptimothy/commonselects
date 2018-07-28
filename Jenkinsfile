pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          agent any
          steps {
            echo 'Build It'
            sshagent()
          }
        }
        stage('ssh') {
          steps {
            sshagent() {
              powershell(script: 'New-Item c:\\AnEmpty.txt -ItemType file', returnStdout: true)
            }

          }
        }
      }
    }
  }
}