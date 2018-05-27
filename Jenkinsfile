pipeline {
  agent any
  tool 'maven-3.5.3'
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
