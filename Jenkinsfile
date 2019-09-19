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

##Información proxy para cada flujo
#export http_proxy=\'http://10.158.122.48:8080/\'
#export https_proxy=\'http://10.158.122.48:8080/\'

mvn -f account-service/pom.xml -Dmaven.test.failure.ignore=true install'''
      }
    }
  }
}