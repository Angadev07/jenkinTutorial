pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git '
https://github.com/Angadev07/jenkinTutorial.git
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }
        stage('Run') {
            steps {
                sh 'mvn exec:java -Dexec.mainClass="com.example.HelloWorld"'
            }
        }
    }
}
