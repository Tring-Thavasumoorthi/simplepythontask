pipeline {
    agent {
        docker { 
            image 'python:3.13.2-alpine3.21' 
        }
    }

    stages {
        stage('Run Python Script') {
            steps {
                sh 'python app.py'  // Execute the Python script inside Docker
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
