pipeline {
  agent {
    node {
      label 'master'
    }
  }
  stage('Gradle Build') {
      steps {
        sh 'gradle clean build -x test -b build-server.gradle'
      }
    }
  }
}
