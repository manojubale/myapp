pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git credentialsId: 'github-token',
                git 'https://github.com/yourusername/myapp.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application..."
                sh 'cp index.html /var/www/html/'
            }
        }
    }
}
