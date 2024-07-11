# This is a demo on deploying AWS EKS in the simplest form using eksctl utility
# you require a simple command to deploy your resources in AWS if your system is #already confiured with AWS. You can add other parameters like the version of your #cluster, the number of nodegroup region etc. e.g of eksctl command: eksctl create #cluster --name my-cluster --region region-code
# You can use fargate to create your nodegroups e.g eksctl create cluster --name 
# my-cluster --regi# on region-code --fargate

eksctl create cluster 
--name my-eks-cluster \
--region us-east-1 \
--nodegroup-name my-eks-nodes \
--node-type t2.micro \
--nodes 2 
