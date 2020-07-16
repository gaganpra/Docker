node{
stage('SCM Checkout'){
       
	checkout scm
	
   }
 
 stage('Build Docker Image'){

	app = docker.build("gaganpra/myimage1")

   }

 stage('Push image'){

	docker.withRegistry('https://registry.hub.docker.com', 'docker-build')
	app.push("${env.BUILD_NUMBER}")
	app.push("latest")
   }
 }
