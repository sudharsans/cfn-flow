pipeline {
  agent any
  stages {
    stage('Source Download') {
      steps {
        git 'https://github.com/apache/maven.git'
      }
    }
    stage('Compile with Maven') {
      steps {
        tool 'maven-3.5.3'
        sh 'mvn package'
      }
    }
  }
}