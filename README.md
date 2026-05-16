# devops-project-k8s
Production-grade Kubernetes on AWS EKS

# Notes
1. What is eksctl?

A command line tool that creates and manages EKS clusters on AWS with one simple command. You write a YAML file describing what you want how many nodes, what size, which region and eksctl goes to AWS and builds everything automatically. Without eksctl you would need to manually create VPC, subnets, IAM roles, security groups and more which takes hours. eksctl does all of that in 15 minutes.

eksctl = tool that builds your Kubernetes cluster on AWS automatically

2. What  is kubectl?

A command line tool that lets you talk to and control your Kubernetes cluster. Once your cluster is running, kubectl is how you deploy apps, check if pods are healthy, read logs, scale up replicas, and manage everything inside the cluster. Think of it like a remote control for your cluster.

kubectl = remote control for your Kubernetes cluster

3. What is helm ?

A package manager for Kubernetes  exactly like npm for Node.js or pip for Python. Instead of managing 10+ YAML files separately for one application, Helm bundles them all into one package called a Chart. You install, upgrade, and rollback entire applications with one command.

Helm = package manager that installs apps on your Kubernetes cluster



# CMD

1. Create cluster  - eksctl create cluster -f cluster/eksctl-config.yaml
2. Delete Cluster -  eksctl delete cluster --name devops-project-cluster --region ap-southeast-2

