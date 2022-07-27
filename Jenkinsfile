@Library('github.com/releaseworks/jenkinslib') _

pipeline {
    agent any
    stages {
        stage('Submit Stack') {
            steps { 
                withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: 'aws-key', usernameVariable: 'AWS_ACCESS_KEY_ID', passwordVariable: 'AWS_SECRET_ACCESS_KEY']]) {
        AWS(sh "aws cloudformation create-stack --stack-name teststack01 --template-body file://Resource.yaml --region 'us-east-1'")
            }
        }
    }
}
