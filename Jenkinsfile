node{
    
stage('SCM Checkout'){
       git credentialsId: 'git-creds', url: 'https://github.com/gaganpra/Docker.git'
   }
 
 stage('Build Docker Image'){
     sh 'docker build -t gaganpr/my-app:2.0.0 .'
   }
 }
