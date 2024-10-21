pipeline {
    agent any
    stages {
        stage('Clonar Repositorio') {
            steps {
                git branch: 'main', url: 'https://github.com/EduardoFoyo/portfolio.git'
            }
        }
        stage('Instalar Dependencias') {
            steps {
                sh 'npm install'
            }
        }
        stage('Construir Proyecto') {
            steps {
                sh 'npm run build'
            }
        }
        stage('Desplegar') {
            steps {
                sh 'npm run deploy'
            }
        }
    }
}
