pipeline {
    agent any

    stages{

        stage ('Build Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("rasolutions/kube-news:${env.BUILD_ID}", '-f ./Dockerfile ./src')
                }
            }
        }
    }
}