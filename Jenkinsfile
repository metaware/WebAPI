pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "dotnet build WebAPI"
            }
        }
        stage('Test') {
            steps {
                sh "dotnet test WebAPI"
            }
        }
        stage('Deploy') {
            steps {
                sh "dotnet publish WebAPI"
            }
        }
    }
}