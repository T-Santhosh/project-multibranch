//Decalartive Pipeline

pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                script{
                     sh 'npm install'
                }
            }
        }
        stage('Docker Build Images') {
            steps {
                script {
                    sh 'docker build -t naresh2603/multi:v2 .'
                    sh 'docker images'
                    sh 'docker ps'
                }
            }
        }
    }
}
