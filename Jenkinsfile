pipeline {
  agent any
  stages {
    stage('enviroment') {
      steps {
        sh '''echo $M2_HOME
export PATH=${PATH}:${M2_HOME}/bin
echo $PATH

mvn --version
'''
      }
    }
    stage('build app') {
      steps {
        sh 'mvn clean package -f account-service/pom.xml'
      }
    }
    stage('build image') {
      steps {
        sh 'docker build -t account-service account-service/.'
      }
    }
  }
}