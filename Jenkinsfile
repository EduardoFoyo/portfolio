pipeline {
    agent any
    stages {
        stage('Clonar Repositorio') {
            steps {
                git 'https://github.com/EduardoFoyo/portfolio'
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
