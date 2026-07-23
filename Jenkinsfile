pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                dir('calculator-app') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage('Test') {
            steps {
                dir('calculator-app') {
                    sh 'mvn test'
                }
            }
        }

        stage('Package') {
            steps {
                dir('calculator-app') {
                    sh 'mvn package'
                }
            }
        }
    }
}
