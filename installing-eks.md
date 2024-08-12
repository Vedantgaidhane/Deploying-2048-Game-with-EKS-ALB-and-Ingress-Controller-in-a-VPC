# Install EKS

Please follow the prerequisites doc before this.

## Install using Fargate

```
eksctl create cluster --name demo-cluster --region us-east-1 --fargate
```

## Delete the cluster

```
eksctl delete cluster --name demo-cluster --region us-east-1



---------------------------------------------------------------------------------------------------------------------------------
# The command aws eks update-kubeconfig --name demo-cluster-1 --region us
east-1 is used to configure the Kubernetes kubectl command-line tool to interact 
with your Amazon EKS cluster.

---
 aws eks update-kubeconfig --name demo-cluster-1 --region us-east-1
---
-----------------------------------------------------------------------------------------------------------------------------------
# 2048 App

## Create Fargate profile

```
eksctl create fargateprofile \
    --cluster demo-cluster \
    --region us-east-1 \
    --name alb-sample-app \
    --namespace game-2048
```

## Deploy the deployment, service and Ingress

```
kubectl apply -f https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.5.4/docs/examples/2048/2048_full.yaml
```


------------------------------------------------------------------------------------------------------------------------------------------
