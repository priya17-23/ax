pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'mvn clean install'
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
        stage('Run') {
            steps {
                bat 'mvn exec:java -Dexec.mainClass=com.example.App'
            }
        }
    }
}
