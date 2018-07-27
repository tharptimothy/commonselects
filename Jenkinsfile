pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          agent any
          steps {
            echo 'Build It'
          }
        }
        stage('Upload to Archive') {
          steps {
            echo 'Uploading To Archive'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        input(message: 'Deploy To Dev', id: '1', ok: '1')
      }
    }
  }
}