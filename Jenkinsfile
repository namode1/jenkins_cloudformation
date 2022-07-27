pipeline {
    agent any
    stages {
        stage('Submit Stack') {
            steps { 
            sh "aws cloudformation create-stack --stack-name teststack --template-body file://Resources.json --region 'us-east-1' --aws-access-key AKIARTWRY2ZYF7ZMZVHT --aws-secret-key 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"
            }
        }
    }
}
