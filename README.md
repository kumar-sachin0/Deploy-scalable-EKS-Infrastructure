**🚀 Highly Available Amazon EKS Cluster with Terraform**
This repository provides a complete Infrastructure-as-Code (IaC) solution to deploy a Highly Available, Secure, and Scalable Amazon EKS Cluster using Terraform. It is designed for production-grade Kubernetes workloads on AWS, following best practices in cloud-native architecture and DevOps.

**📌 Key Features**
Multi-AZ High Availability: EKS control plane and worker nodes span multiple Availability Zones.
Secure Networking: Custom VPC with public/private subnets, NAT gateways, and routing.
IAM Integration: Fine-grained IAM roles and policies for Kubernetes components and users.
Managed Node Groups: Auto-scaling worker nodes with lifecycle management.
Observability: Logging and monitoring enabled for cluster insights.
Remote State Management: S3 backend with DynamoDB for state locking and team collaboration.
🛠️ Technologies Used
Terraform (v1.x)
AWS EKS
Amazon VPC, IAM, S3, DynamoDB
Kubernetes
kubectl, aws-cli


**📋 Architecture Overview**

+---------------------------+
|     Terraform Scripts     |
+---------------------------+
            |
            v
+---------------------------+
|     AWS Infrastructure    |
|  - VPC (Multi-AZ)         |
|  - EKS Control Plane      |
|  - Managed Node Groups    |
|  - IAM Roles & Policies   |
|  - S3 + DynamoDB Backend  |
+---------------------------+

**✅ Benefits**
By following this setup, your EKS cluster will be:

Highly Available: Resilient across multiple Availability Zones.
Secure: IAM and network policies enforce least privilege.
Scalable: Auto-scaling node groups adapt to workload demands.
Maintainable: Fully managed via Terraform for repeatability and version control.
🚀 Getting Started
Clone the Repository


Configure AWS Credentials


Initialize Terraform


Plan and Apply


**📎 Prerequisites**
AWS Account with appropriate permissions
Terraform CLI installed
kubectl and aws-cli configured
Backend S3 bucket and DynamoDB table (optional but recommended)


**📈 Future Enhancements**
Add support for Fargate profiles
Integrate with GitOps tools (e.g., ArgoCD, Flux)
Enable service mesh (e.g., Istio, Linkerd)
Add Helm chart deployments
