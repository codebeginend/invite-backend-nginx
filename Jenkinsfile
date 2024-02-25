pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Шаги сборки проекта
                sh 'echo "Building the project"'
                sh 'docker-compose build'
            }
        }

        stage('Test') {
            steps {
                // Шаги тестирования
                sh 'echo "Running tests"'
            }
        }

        stage('Deploy') {
            steps {
                // Шаги развертывания
                sh 'echo "Deploying the project"'
                sh 'docker-compose up -d'
            }
        }
    }
}
