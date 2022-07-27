pipeline {
    agent any
    stages {
        stage('Submit Stack') {
            steps { 
            sh "aws cloudformation create-stack --stack-name teststack01 --template-body file://Resource.yaml --region 'us-east-1'"
            }
        }
    }
}
