# python-helloworld-deployment
    Step 1: Docker Login:
      "docker login"
     > Purpose: Authenticates you with Docker Hub (or another Docker registry) using yourcredentials.
		 > Result: Login Succeeded indicates you are now authenticated and can push/pull images from y

		Step 2: Docker Build (Successful Attempt):
					"docker build -t sample ."
		 			"docker build -t username/image ."
			> Purpose: Builds a Docker image from a Dockerfile in the current directory (.).
	 
		Step 3: Apply Kubernetes Deployment:
					"kubectl apply -f deployment.yml"
		 	> Purpose: Applies the Kubernetes deployment configuration defined in deployment.yml
		
		 		Result:
		 				"deployment.apps/python-helloworld-deployment created"

		Step 4: Check Kubernetes Pods:
					"kubectl get pods"
		 
				> Purpose: Lists all running pods in the current Kubernetes namespace.

				Result:
						> Multiple pods are listed, including those for bharathi and python-helloworld-deployment.
						> The python-helloworld-deployment pods are running successfully (READY 1/1 and STATUS Running).
			
				---------------------------------------------------------------------------------------------------------------		
			
