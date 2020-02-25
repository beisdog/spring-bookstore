pipeline {
  agent {
    docker {
      image 'maven:3-alpine'
      args '-v /Users/dbe/.m2:/root/.m2'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'mvnw clean build'
      }
    }

  }
}