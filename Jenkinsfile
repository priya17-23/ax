pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'mvn clean install exec:java -Dexec.mainClass=com.example.c'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }
    }
}
