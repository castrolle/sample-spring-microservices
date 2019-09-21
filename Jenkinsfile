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
  }
}