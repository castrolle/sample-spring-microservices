pipeline {
  agent any
  stages {
    stage('pull image') {
      steps {
        sh 'docker pull maven:3.3.9-jdk-8'
      }
    }
    stage('mvn version') {
      steps {
        sh 'mvn --version'
      }
    }
  }
}