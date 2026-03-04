pipeline {
    agent any

    tools {
        nodejs "Node18"
    }

    stages {

        stage('Checkout Code') {
            steps {
                git 'https://github.com/TU_USUARIO/TU_REPO.git'
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