# Website Deployment on AWS

This section demonstrates the infrastructure provisioning and application deployment workflow used for the project.

## Terraform Infrastructure

Terraform was used to initialize, validate, and provision the required AWS infrastructure.

![Terraform Configuration](./kubernetes_main.tf_created.jpg)

## Infrastructure Provisioning

The Terraform configuration was successfully applied to provision the required infrastructure.

![Terraform Apply](./kubernetes_main.tf_apply.jpg)

## Application Deployment

The website application was deployed to the Kubernetes environment running on AWS.

![Application Deployment](./application_localhost.jpg)

## Application Running

The deployed website was successfully accessed and verified.

![Application Running](./website-app_pod_running.jpg)

![Application Running](./application_running.jpg)

## Deployment Workflow

The overall deployment process involved:

**Terraform → AWS Infrastructure → EKS/Kubernetes → Docker Container → Website Application**
