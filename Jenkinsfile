pipeline {
    agent {
        docker {
            image 'gradle/gradle-enterprise-test-distribution-agent'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'gradle clean build -x test -b build-server.gradle'
            }
        }
    }
}
