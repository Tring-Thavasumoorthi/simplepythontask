pipeline {
    agent { label 'fargate' } 
    stages {
        stage('Run Node Script') {
            steps {
                sh 'node app.js'
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
