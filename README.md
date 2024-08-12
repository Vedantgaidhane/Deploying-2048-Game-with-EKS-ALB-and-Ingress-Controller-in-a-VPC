# Deploying-2048-Game-with-EKS-ALB-and-Ingress-Controller-in-a-VPC

In this project, a comprehensive VPC architecture was developed and deployed to host the popular 2048 game using Amazon Elastic Kubernetes Service (EKS). The key components and steps involved in this deployment are as follows:

Key Components:
VPC Architecture: Created a Virtual Private Cloud (VPC) with both public and private subnets to ensure a secure and scalable network environment.
Amazon EKS: Deployed an EKS cluster to manage and orchestrate the Kubernetes-based application.
Application Load Balancer (ALB): Implemented an ALB to handle incoming traffic from the public subnet.
Configured the ALB to direct traffic to the appropriate cluster IP services within the private subnet.
Ingress Controller: Set up an Ingress Controller to manage the routing of traffic to the application pods.
Ensured efficient load balancing and traffic management to optimize application performance.
Project Highlights:
Network Security and Segmentation: The VPC setup, incorporating both public and private subnets, ensured a secure and segmented network, isolating critical components for enhanced security.
Scalable and Efficient Traffic Management: The use of ALB and Ingress Controller facilitated effective traffic routing and load balancing, providing a seamless user experience and maintaining high availability.
Container Orchestration: Leveraged Amazon EKS for robust container orchestration, enabling efficient deployment, scaling, and management of the 2048 game application.

This project demonstrates a sophisticated approach to deploying a web application in a cloud-native environment, utilizing advanced networking, load balancing, and container orchestration techniques to ensure optimal performance and scalability.
