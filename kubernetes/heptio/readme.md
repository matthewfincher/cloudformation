# Heptio Kubernetes

- VPC with public and private two subnets
- In the public subnet, a Linux bastion and ELB
- In the private subnet, a Kubernetes cluster on Ubuntu 16.04 LTS. 
- One master node EC2 instance and 1-20 EC2 worker node instances in an Auto Scaling group
- kubeadm for cluster administration
- Docker for the container runtime
- Calico or Weave for networking between pods
- Security group for bastion SSH access and inter-node connectivity 
