# Project

This simple NodeJS app needs to work with Mongo DB.

Design a GitHub Actions workflow to achieve CI/CD.

## Description

- Build the app into a Container image
- Use Container Registry to manage the images
- Deploy your built image to a Kubernetes cluster
- Expose your service to the Internet
- Use Grafana to monitor performance metrics

## Architecture

![image](images/Screenshot%202023-05-14%20at%2010.36.28%20am.png)

1- Change application source code.

2- Commit code to GitHub.

3- Continuous Integration Trigger to Jenkins.

4- Jenkins triggers a build job using Azure Container Service (AKS) for a dynamic build agent.

5- Jenkins builds and pushes Docker container Azure Container Registry.

6- Jenkins deploys new containerized app to Kubernetes on Azure Container Service (AKS) backed by Azure Cosmos DB.

7- Grafana displays visualization of infrastructure and application metrics via Azure Monitor.

8- Monitor application and make improvements.

## Secret and variables

Secret:
ACS_PASSWD=

ACS_USERNAME=

AZURE_CLIENT_ID=

AZURE_SUBSCRIPTION_ID=

AZURE_TENANT_ID=

MONGODB_URI=

Variables
ACS_LOGIN_SERVER=

AKS_CLUSTER_NAME=

AZURE_CONTAINER_REGISTRY=

IMAGE_NAME=

RESOURCE_GROUP=

Sample

![image](images/Screenshot%202023-05-14%20at%209.58.35%20pm.png)
![image](images/Screenshot%202023-05-14%20at%209.58.28%20pm.png)

## Output

![image](images/Screenshot%202023-05-14%20at%208.31.23%20pm.png)
![image](images/Screenshot%202023-05-14%20at%209.49.50%20pm.png)
![image](images/Screenshot%202023-05-14%20at%209.50.00%20pm.png)
![image](images/Screenshot%202023-05-14%20at%209.50.07%20pm.png)
![image](images/Screenshot%202023-05-14%20at%209.49.50%20pm.png)
![image](images/Screenshot%202023-05-14%20at%209.48.58%20pm.png)
![image](images/Screenshot%202023-05-14%20at%209.49.10%20pm.png)
![image](images/Screenshot%202023-05-14%20at%209.49.23%20pm.png)
![image](images/Screenshot%202023-05-14%20at%209.49.41%20pm.png)
![image](images/Screenshot%202023-05-14%20at%209.49.32%20pm.png)
