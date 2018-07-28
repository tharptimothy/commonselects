pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        sleep 2
      }
    }
  }
  environment {
    Development = 'Dev'
    Production = 'Prod'
    Staging = 'QC'
  }
}