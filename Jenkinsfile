pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/timgio26/customerDataPlatform_react.git', branch: 'main'
            }
        }
        stage('Build') {
            steps {
                sh 'docker build -t frontend-image .'
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
