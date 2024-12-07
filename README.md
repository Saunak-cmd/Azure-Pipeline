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

Artifact Creation:​

Push the manifests folder (containing Kubernetes deployment and service YAML files) as an artifact in the pipeline for reuse in subsequent stages.​

Update deployment and service manifest files to dynamically use namespaces (dev or prod) based on pipeline variables.​

Streamline deployments by enabling reusable artifacts and environment-specific configurations.​

Fine-Tuning Pipelines:​

Move deployment processes to a release pipeline.​

Add a 3-minute gate wait in pipelines.​

Update deployment/service files to utilize namespaces as variables (dev and prod).​

Release Pipeline:​

Set up a release pipeline for production deployments.​

Deploy to the production namespace using separate Load Balancer IPs for development and production environments.​