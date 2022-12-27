pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {
        stage('Build') {
            steps {
                sh 'docker info'
                sh 'mvn --version'
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}