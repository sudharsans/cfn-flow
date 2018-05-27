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
        sh '
        tool 'maven-3.5.3'
        mvn package
        '
      }
    }
  }
}
