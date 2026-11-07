

# ClusterIP Service Lab

## Objective

Expose an application internally within the Kubernetes cluster using a ClusterIP service.

## Components

- Deployment
- Service (ClusterIP)

## Create Resources


kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

Verify
Shell
kubectl get pods
kubectl get svc

Expected:

Plain Text
clusterip-service ClusterIP
Test
Shell
kubectl run busybox --image=busybox -it --rm -- sh

Inside Pod:

Shell
wget -qO- http://clusterip-service

Expected:

HTML
Welcome to nginx!
Cleanup
Shell
kubectl delete -f .


