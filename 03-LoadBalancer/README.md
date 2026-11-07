# LoadBalancer Service Lab

## Objective

Learn how to expose applications externally using a LoadBalancer service.

## Components

- Deployment
- LoadBalancer Service

## Deploy

kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

## Start Tunnel

minikube tunnel

## Verify

kubectl get svc

Expected:

External IP Assigned

## Test

curl http://<external-ip>

Expected Result:

Welcome to nginx!

## Cleanup

kubectl delete -f .
