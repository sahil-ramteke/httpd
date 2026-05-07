pipeline{
    agent any
    stages{
        stage('clone repo'){
            steps{
                sh 'rm -rf *'
                git branch: 'main', url: 'https://github.com/sahil-ramteke/repository2'
            }
        }
        stage('copy file'){
            steps{
                sh 'cp /root/.jenkins/workspace/job-2/index.html /var/www/html/'
            }
            }
        }
    }
