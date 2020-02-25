pipeline {
  agent {
    docker {
      image 'maven:3-alpine'
      args '-v /root/.m2:/Users/dbe/.m2'
    }

  }
  stages {
    stage('build') {
      steps {
        sh './gradlew build'
      }
    }

  }
}