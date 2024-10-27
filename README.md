# MongoDB and Mongo-Express Kubernetes Deployment on EKS

This project deploys MongoDB and Mongo-Express on an Amazon EKS cluster for practicing Kubernetes resource management. The deployment utilizes core Kubernetes components, such as ConfigMaps, Secrets, Deployments, Services, Load Balancers, and Ingress.

## Project Overview

- **MongoDB**: A NoSQL database for storing application data.
- **Mongo-Express**: A web-based MongoDB admin interface, which allows easy access to MongoDB data.

## Kubernetes Components Used

- **ConfigMap**: Stores configuration data for MongoDB and Mongo-Express, such as environment variables.
- **Secret**: Manages sensitive information like database credentials.
- **Deployment**: Manages the deployment and scaling of MongoDB and Mongo-Express applications.
- **Service**: Exposes MongoDB and Mongo-Express within the cluster.
- **Load Balancer**: Used for external access to Mongo-Express.
- **Ingress**: Provides routing and access control for external traffic to Mongo-Express.

## Project Structure

| File Name             | Description |
|-----------------------|-------------|
| `mongo.yaml`          | MongoDB Deployment and Service configuration. |
| `mongo-configmap.yaml`| ConfigMap for MongoDB environment variables. |
| `mongo-express.yaml`  | Mongo-Express Deployment and Service configuration. |
| `mongo-headless.yaml` | Headless Service for MongoDB, enabling internal communication within the cluster. |
| `mongo-secret.yaml`   | Secret containing MongoDB credentials. |
| `mysql-configmap.yaml`| Additional ConfigMap for MySQL (if required for future expansion). |

## Prerequisites

- **Amazon EKS Cluster**: Ensure you have an EKS cluster set up with kubectl access.
- **kubectl**: Command-line tool for interacting with the Kubernetes cluster.
- **AWS CLI**: Used for EKS authentication.

## Deployment Steps

1. **Clone the Repository**:

   ```bash
   git clone git@github.com:Dakuchi/kubernetes.git
