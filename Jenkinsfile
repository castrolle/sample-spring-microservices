pipeline {
  agent any
  stages {
    stage('ls') {
      steps {
        sh '''ls
#mvn --help
docker ps'''
      }
    }
  }
}