# NodePort Service Lab

## Objective

Learn how to expose applications outside the Kubernetes cluster using a NodePort service.

## Components

- Deployment
- NodePort Service

## Deploy

kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

## Verify

kubectl get svc

Expected:

Type = NodePort

## Test

minikube service nodeport-service --url

Open the displayed URL in a browser.

Expected Result:

Welcome to nginx!

## Cleanup

kubectl delete -f .
