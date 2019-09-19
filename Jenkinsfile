pipeline {
  agent {
    docker {
      image 'maven:3.3.9-jdk-8'
    }

  }
  stages {
    stage('ls') {
      steps {
        sh 'ls'
      }
    }
  }
}