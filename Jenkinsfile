pipeline {
    agent any

    tools {
        nodejs "Node18"
    }

    stages {

        stage('Checkout Code') {
            steps {
                git 'https://github.com/ezabalat/devops-testing.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'npm test'
            }
        }

        stage('Deploy Simulation') {
            steps {
                echo '🚀 Deploy exitoso'
            }
        }

    }
}