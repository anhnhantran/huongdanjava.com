pipeline {
  agent any
  stages {
    stage('Clean Directory') {
      steps {
        sh 'rm -rf *'
      }
    }

    stage('Clone Git') {
      steps {
        sh 'git clone https://github.com/anhnhantran/huongdanjava.com.git'
      }
    }

    stage('Build') {
      steps {
        sh 'mvn clean install -f spring-helloworld/pom.xml'
      }
    }

  }
}