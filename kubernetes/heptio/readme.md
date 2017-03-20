# Heptio Kubernetes

- VPC in Single AZ with public and private subnets
- Linux bastion and ELB in public subnet
- Private subnet:
  - a Kubernetes cluster on Ubuntu 16.04 LTS. 
  - One master node EC2 instance with automatic recover 
  - 1-20 EC2 worker node instances in an Auto Scaling group
- kubeadm for cluster administration
- Docker for the container runtime
- Calico or Weave for pod networking
- Security group:
  - port 22 for bastion SSH access 
  - port 6443 for HTTPS access to API
  - all ports for inter-node connectivity
- all nodes are Ubuntu 16.04 LTS; the base image is a custom AMI based on Ubuntu 16.04
