# Install EKS

Please follow the prerequisites doc before this.

## Install a EKS cluster with EKSCTL

```
eksctl create cluster --name demo-cluster --region us-east-1 
```
## Run following command to update the kubeconfig
```
aws eks update-kubeconfig --region <region-name> --name <cluster-name>
```

## Delete the cluster

```
eksctl delete cluster --name demo-cluster --region us-east-1
```
