pipeline {
agent { label 'linux-agent' }
stages {
stage('Build') {
steps {
sh 'mvn clean compile'
}
}
stage('Test') {
steps {
sh 'mvn test'
}
}
stage('Package') {
steps {
sh 'mvn package'
}
}
}
}
