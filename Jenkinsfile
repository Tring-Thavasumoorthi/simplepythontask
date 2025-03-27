pipeline {
    agent { label 'fargateagent' }  https://github.com/Tring-Thavasumoorthi/simplepythontask/blob/main/Jenkinsfile

    stages {
        stage('Run Python Script') {
            steps {
                sh 'python3 app.py'
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
