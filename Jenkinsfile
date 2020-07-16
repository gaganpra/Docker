node{
stage('SCM Checkout'){
       
	checkout scm
	
   }
 
 stage('Build Docker Image'){

	app = docker.build(gaganpr/testimage123)

   }

 stage('Push image'){

	docker.withRegistry('https://registry.hub.docker.com', 'Docker_Build')
	app.push("${env.BUILD_NUMBER}")
	app.push("latest")
   }
 }
