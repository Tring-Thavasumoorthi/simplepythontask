pipeline {
    agent any

    stages {
        stage('Run Python Script') {
            steps {
                sh 'docker run --rm -v $PWD:/app -w /app python:3.13.2-alpine3.21 python app.py'
            }
        }
    }

    post {
        success {
            echo '🎉 Pipeline executed successfully!'
        }
        failure {
            echo '❌ Pipeline failed!'
        }
    }
}
