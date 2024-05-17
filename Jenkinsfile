pipeline {
    agent any
    stages {
        stage('Welcome') {
            steps {
                echo 'Jenkins'
            }
        }    
        stage('Checkout') {
            steps {
                git 'https://github.com/Vivekrsg/Jenkins.git'
            }
        }
        stage('build') {
            steps {
                echo 'Skipping build'
            }
        }    
        stage('test') {
            steps {
                echo 'Skipping Test'
            }
        }    
        stage('deploy') {
            steps {
                sh 'sudo apt get update && sudo get install -y ngnix'
                sh 'sudo cp index.html /var/www/html/'
                sh 'sudo systemctl restart nginx'
            }
        }    
    }   
}