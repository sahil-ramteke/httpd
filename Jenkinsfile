pipeline{
    agent any
    stages{
        stage('clone repo'){
            steps{
                sh 'rm -rf *'
                git branch: 'main', url: 'https://github.com/sahil-ramteke/repository3'
            }
        }
        stage('copy file'){
            steps{
                sh 'cp /root/.jenkins/workspace/job-3/index.html /var/www/html/'
            }
            }
        }
    }
