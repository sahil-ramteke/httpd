pipeline{
    agent any
    stages{
        stage('clone repo'){
            sh 'rm -rf *'
            git branch: 'main', url: 'https://github.com/sahil-ramteke/repository3'
        }
        stage('copy file'){
            sh 'cp repository1/index.html /var/www/html/'
        }
    }
}
