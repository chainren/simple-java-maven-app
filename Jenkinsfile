pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v C:/Users/Administrator2/.m2/repository:/root.m2'
        }
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}