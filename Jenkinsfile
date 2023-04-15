pipeline {
    agent any

    stages {

        stage ('Build docker iamge') {
            steps {
                script {
                    dockerapp = docker.build("meurerfagner/kub-news:${env.BUILD_ID}",'-f .src/Dockerfile ./src')
                }
            }
        }
    }
}