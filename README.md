This module is to deploy sample `hello world` application to Kubernetes cluster we created using sample-base-infra repo.

Local development:

1. Install docker and kubectl.
2. Clone this repo and cd to deploy-k8s directory.
3. Run docker build command.
4. Push the docker image to ECR repo.
5. cd to deploy-k8s directory.
6. Edit app.yaml, replace ACCOUNT_NAME, REGION and ECR_REPO_NAME with valid values.
7. Apply the yaml file to EKS cluster.
8. Access the application via public load balancer DNS.

Circle Execution:

1. Edit app.yaml, replace ACCOUNT_NAME, REGION and ECR_REPO_NAME with valid values.
2. Edit .circleci/config.yaml and provide valid values for parameters.
3. Push the code to github.com.
4. Setup Project on app.circleci.com.
5. Setup Environment variables for AWS auth in the project.

Happy building!