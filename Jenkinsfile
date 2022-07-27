pipeline {
    agent any
    stages {
        stage('Submit Stack') {
            steps { 
            sh "aws cloudformation create-stack --stack-name teststack --template-body file://Resources.json --region 'us-east-1' --aws-access-key $AWS_ACCESS_KEY_ID --aws-secret-key $AWS_SECRET_ACCESS_KEY"
            }
        }
    }
}
