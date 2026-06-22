pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/abhinav150487/django-todo-cicd.git'
            }
        }

        stage('Build') {
            steps {
                sh 'docker build -t todo-app .'
            }
        }

        stage('Test') {
            steps {
                sh 'docker run --rm todo-app python manage.py test'
            }
        }

        stage('Deploy') {
            steps {
                sh 'docker run -d -p 8000:8000 --name todo-app-container todo-app'
            }
        }
    }
}
