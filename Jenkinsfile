pipeline {
    agent any
    stages {
        stage('---clone repo &&&&&&&& clean it---') {
            steps {
                sh "rm -rf my-app"
                sh "git clone https://github.com/devopsafroz/my-app.git"
                sh "mvn clean -f my-app"
            }
        }
        stage('--test-- and testing -----') {
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
