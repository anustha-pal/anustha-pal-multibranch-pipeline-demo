pipeline {
    agent any
    stages {
        stage('Build for dev') {
            steps {
                script {
                    echo "Building branch: ${env.BRANCH_NAME}"
                }
            }
        }
        stage('Test in dev') {
            steps {
                sh 'bash app/hello.sh'
            }
        }
        stage('Deploying in dev') {
            steps {
                echo "Deploying branch: ${env.BRANCH_NAME}"
            }
        }
    }
}
