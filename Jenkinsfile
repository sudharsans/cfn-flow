pipeline {
  agent any
    tools {
        maven 'maven-3.5.3' 
        jdk 'jdk'
    }
  stages {
    stage('Source Download') {
      steps {
        git 'https://github.com/apache/maven.git'
      }
    }
    stage('Compile with Maven') {
      steps {
        sh 'mvn package'
      }
    }
  }
}
