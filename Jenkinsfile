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

    stage('Deploy') {
      steps {
        sh 'rsync -avz -e "ssh" ./dist/my-dream-app/* root@167.71.228.123:/var/www/html/'
      }
    }

  }
}