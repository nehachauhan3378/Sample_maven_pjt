pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                withMaven(maven : 'Maven') {
                    bat 'mvn clean install'
                }
            }
        }
        stage('Test') {
            steps {
                withMaven(maven : 'Maven') {
                    bat 'mvn test'
                }
            }
        }
    }
}
