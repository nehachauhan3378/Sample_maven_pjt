pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                withMaven(maven: 'Maven') {
                echo 'Building..'
                sh 'mvn clean install'
                }
            }
        }
        stage('Test') {
            steps {
                withMaven(maven: 'Maven') {
                echo 'Testing..'
                sh 'mvn test'
                }
            }
        }
    }
}
