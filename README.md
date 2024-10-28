# kubernetes-objects

##Objectives
Create a Kubernetes Service
Use various kubectl commands
Deploy a StatefulSet for managing stateful applications
Implement a DaemonSet for running a single pod on all nodes


# Setup Environment
Open a terminal window using the menu: Terminal > New Terminal.

<h2>Step 1: Verify kubectl Version</h2>
Before proceeding, ensure that you have kubectl installed and properly configured. To check the version of kubectl, run the following command:

>
>
>     kubectl version


![image](https://github.com/user-attachments/assets/3e7cdeb1-f0cf-476b-ba28-3946c11fa008)


<h2>Task 1: Create a Kubernetes Service using nginx image</h2>

A popular open-source web server, nginx is known for its high performance, stability, and low resource usage. It can also function as a reverse proxy, load balancer, and HTTP cache.

Creating a Kubernetes Service using an nginx image involves setting up a networking layer that allows other components within the Kubernetes cluster or external users to access the nginx application running in pods. To run nginx as a service in Kubernetes, you can follow these steps:

<b>Create a Deployment named my-deployment1 using the nginx image</b>

>
>
>      kubectl create deployment my-deployment1 --image=nginx

![image](https://github.com/user-attachments/assets/91a7a3bb-360f-4ddd-8a65-3dc8aa2914e3)

kubectl: The command-line tool for interacting with the Kubernetes API.

create deployment: Tells Kubernetes that you want to create a new Deployment. A Deployment is a Kubernetes object that manages a set of replicated Pods, ensuring that the specified number of replicas are running and updated.

my-deployment1: It is the name of the Deployment being created. In this case, the Deployment is named my-deployment1.

--image=nginx: It specifies the container image used for the Pods managed by this Deployment. The nginx image is a popular web server and reverse proxy server.

It creates a Deployment named my-deployment1 that uses the nginx image. Deployments manage the rollout and scaling of applications.
