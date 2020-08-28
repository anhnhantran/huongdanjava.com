pipeline {
  agent any
  stages {
    stage('Clone Git') {
      steps {
        sh '''rm -rf huongdanjava_master
git clone https://github.com/anhnhantran/huongdanjava.com.git'''
      }
    }

    stage('Build') {
      steps {
        sh 'mvn clean install -f huongdanjava.com_master/spring-boot-internalresourceviewresolver/pom.xml'
      }
    }

  }
}