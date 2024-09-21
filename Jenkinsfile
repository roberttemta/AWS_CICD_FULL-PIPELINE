 pipeline{

    agent any

   stages{
    stage('git Checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/roberttemta/AWS_CICD_FULL-PIPELINE.git'
            }
        }
        stage('test'){
            steps{
                sh 'echo test'
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