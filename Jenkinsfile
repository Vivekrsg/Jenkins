pipeline {
   agent any
    stages {
       stage('Welcome') {
           steps {
               echo 'All good! Jenkin Task'
           }
       }
        stage('checkout') {
           steps {
               git https://github.com/Vivekrsg/Jenkins.git
           }
       }
       stage('build') {
           steps {
               echo 'skipping build'
           }
       }
       stage('test') {
           steps {
               echo 'skipping test'
           }
       }
       stage('deploy') {
           steps {
               sh 'sudo apt-get update && sudo apt-get install -y nginx'
               sh 'sudo cp index.html /var/www/html/'
               sh 'sudo systemctl restart nginx'
           }
       }
   }
}
