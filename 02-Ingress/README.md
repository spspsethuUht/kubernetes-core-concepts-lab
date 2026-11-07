# Ingress Lab

## Objective

Learn how to route HTTP traffic using Kubernetes Ingress.

## Enable Ingress

minikube addons enable ingress

## Deploy

kubectl apply -f deployment.yaml

kubectl apply -f service.yaml

kubectl apply -f ingress.yaml

## Verify

kubectl get ingress

## Configure Host Entry

Add:

127.0.0.1 myapp.local

to the hosts file.

## Test

Open:

http://myapp.local

Expected Result:

Welcome to nginx!

## Cleanup

kubectl delete -f .
