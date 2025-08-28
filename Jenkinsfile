pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    echo "Building branch: ${env.BRANCH_NAME}"
                }
            }
        }
        stage('Test') {
            steps {
                sh 'bash app/hello.sh'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying branch: ${env.BRANCH_NAME}"
            }
        }
    }
}
