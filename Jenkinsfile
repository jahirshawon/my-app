pipeline {
    agent any
    stages {
        stage('clone repo and clean') {
            steps {
                sh "git clone https://github.com/jahirshawon/my-app.git"
                sh " mvn clean -f my-app"
            }
        }
        stage('--test--') {
            steps {
                sh "mvn test -f my-app"
            }
        }
        stage('--package--') {
            steps {
                sh "mvn package -f my-app"
            }
        }
    }
}
