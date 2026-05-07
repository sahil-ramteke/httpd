pipeline{
    agent any
    stages{
        stage('install httpd'){
            steps{
                sh 'yum install httpd -y'
                sh 'systemctl start httpd'
                sh 'systemctl enable httpd'
            }
        }
        stage('make file'){
            steps{
                sh 'echo "This is index file" >> /var/www/html/index.html'
                sh 'chmod -R 777 /var/www/html/'
            }
        }
    }
}
