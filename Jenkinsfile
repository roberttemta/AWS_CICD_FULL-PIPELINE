 pipeline{

    agent any

    environment {
        BRANCH_NAME = 'main'
        GIT_URL = 'https://github.com/roberttemta/AWS_CICD_FULL-PIPELINE.git'
        IMAGE_TAG = "roberttemta/awscicd"
        IMAGE_VERSION = ${BUILD_NUMBER}
    }

   stages{
    stage('git Checkout'){
            steps{
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }
        stage('Docker Build'){
            steps{
                sh 'docker build -t "${IMAGE_TAG}":"${IMAGE_VERSION}" .'
                sh 'docker images'
            }
        }

        stage('pwd command'){
            steps{
                sh 'pwd'
            }
        }

        stage('ls command'){
            steps{
                sh 'ls'
            }
        }
        
    }
}