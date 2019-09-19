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
    stage('') {
      steps {
        sh '''echo PATH=${PATH}
echo M2_HOME=${M2_HOME}
'''
      }
    }
  }
}