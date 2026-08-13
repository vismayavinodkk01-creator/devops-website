pipeline{
    agent any
    stages{
        stage('checkout'){
            steps{
                sh '''
                rm -rf *
                git clone https://github.com/vismayavinodkk01-creator/devops-website.git
                '''
            }
        }
        stage('deploy'){
            steps{
                sh '''
                pwd
                rm -rf /var/www/html/*
                cp -r devops-website/* /var/www/html
                '''
            }
        }
    }
}
