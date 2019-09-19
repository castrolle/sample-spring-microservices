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
    stage('maven') {
      steps {
        sh '''#more account-service/pom.xml
#mvn clean package -f account-service/pom.xml
mvn -f account-service/pom.xml -Dmaven.test.failure.ignore=true install'''
      }
    }
  }
}