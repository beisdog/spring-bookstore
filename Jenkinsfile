pipeline {
  agent {
    docker {
      args '-v /Users/dbe/.m2:/root/.m2'
      image 'maven:3.6.3-jdk-11'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }

    stage('test') {
      steps {
        sh 'mvn test'
      }
    }

  }
}