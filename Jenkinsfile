pipeline {
  agent any
    stages {
        stage('Submit Stack') {
            steps { 
            sh "aws cloudformation create-stack --stack-name teststack --template-body file://Resources.yaml --region 'us-east-1"
                
            }
        }
    }
}
