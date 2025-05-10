pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/techrewk/new_repa.git'
            }
        }

        stage('Build with Maven') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the app...'
                // Put your deployment logic here
            }
        }
    }
}

