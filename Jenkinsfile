pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {
        stage('Build') {
            steps {
                 docker.image('maven:3.3.3').inside {
                        sh 'mvn --version'
                      }
            }
        }
    }
}