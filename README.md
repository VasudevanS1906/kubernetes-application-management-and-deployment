# Kubernetes-Application-Management-and-Deployment
Deployed and managed a containerized Nginx web application on a Kubernetes cluster, utilizing manifests to create Deployments, Services, and ConfigMaps. Scaled the application from 2 to 4 replicas, performed rolling updates with zero downtime, and troubleshot issues using kubectl commands, demonstrating proficiency in essential Kubernetes concepts and operations.

# Screenshot

The following screenshot shows the successful deployment of the Kubernetes cluster:

![Screenshot](kubernetes_success_msg.png)

The output confirms that the nginx-deployment has multiple replicas (Pods) running, the Deployment was updated with the latest configuration, and the nginx-service was created to expose the application

# Prerequisites

Before getting started, make sure you have the following prerequisites installed:

1.Git

2.Kubernetes cluster (local or remote)

# Getting Started

To get started with this project, follow these steps:

Clone the repository:

      git clone https://github.com/VasudevanS1906/kubernetes-application-management-and-deployment.git

Change to the project directory:

      cd kubernetes-web-app-deployment

# Usage

This project provides hands-on experience with deploying and managing a web application using Kubernetes. Here's how you can use it:

1. Set up a Kubernetes Cluster

Set up a Kubernetes cluster locally or on a cloud platform.

2. Deploy the Application

To deploy the web application, run the following command:

      kubectl apply -f .
This command will apply all the necessary resources (Deployment, Service, etc.) to the cluster.

3. Scale the Application

You can scale the application by modifying the number of replicas in the Deployment. For example:

      kubectl scale deployment/app --replicas=5

4. Access the Application
Once the application is deployed, you can access it by exposing the Service. 

            kubectl port-forward service/app 8080:80

5. Monitoring and Troubleshooting

For monitoring and troubleshooting purposes, you can use various Kubernetes commands and tools, such as kubectl get, kubectl describe, kubectl logs, and kubectl exec.

6. Cleanup

When you're done, you can delete the resources created by this project by running the following command:

      kubectl delete service,deployment app

# Support and Contact

If you have any questions, please feel free to contact me at [vasudevanswornampillai@gmail.com].

# License

This project is licensed under the **Apache 2.0 License**.

# Share with the community

If you find this project interesting or helpful, don't hesitate to share with your community! Let's learn and grow together!

# Conclusion

In this project, we’ve deployed and managed a containerized Nginx web application on a Kubernetes cluster, utilizing manifests to create Deployments, Services and ConfigMaps. The model, a beacon of performance, awaits those go into the beautiful world of Devops.
