pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        nodejs('Angular') {
          sh '''npm install
'''
          sh 'ng build'
        }

      }
    }

  }
}