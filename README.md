Code Development:​

Develop features on the Dev branch using Visual Studio Code.​

Commit changes locally and push them to Azure Repos.​

Application Selection and Deployment:​

Choose a sample application (e.g., a Python Flask app with Redis) and create or clone its repository in Azure Repos.​

Containerization:​

Create a Dockerfile for the application, build the Docker image locally, and perform testing.​

Push the tagged Docker image to the Azure Container Registry (ACR).​

Deploy the application components to a AKS cluster on Azure using Azure DevOps pipelines:​

Apply Kubernetes namespace in the manifests dynamically based on pipeline variables.​

Leverage Azure Resource Manager service connection for secure integration.​

Application Deployment:​

Deploy the application manifests, including Python-based services and Redis configurations.​

Utilize the container image built in the previous stage and push it to Azure Container Registry (ACR).​

Deployment Verification:​

Run a script to verify that Kubernetes pods and services are running as expected.​

Fetch the external IP of the Python app service and test connectivity using curl​

Approvals:​

Include manual approval stage for sensitive actions, such as deleting deployments or services.​