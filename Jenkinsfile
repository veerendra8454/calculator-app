pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                dir('calculater-app') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage('Test') {
            steps {
                dir('calculater-app') {
                    sh 'mvn test'
                }
            }
        }

        stage('Package') {
            steps {
                dir('calculater-app') {
                    sh 'mvn package'
                }
            }
        }
    }
}
