pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                withMaven(maven : 'Maven') {
                    sh 'mvn clean install'
                }
            }
        }
        stage('Test') {
            steps {
                withMaven(maven : 'Maven') {
                    sh 'mvn test'
                }
            }
        }
    }
}
