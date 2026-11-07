# LoadBalancer Notes

## What is LoadBalancer?

LoadBalancer provides external access to applications running inside Kubernetes.

Cloud providers automatically create and manage the load balancer.

## Examples

- AWS Load Balancer
- Azure Load Balancer
- Google Cloud Load Balancer

## Traffic Flow

Client

↓

Load Balancer

↓

Service

↓

Pod

## Minikube Requirement

Minikube requires:

minikube tunnel

## Key Takeaway

LoadBalancer is the preferred method for exposing production applications in cloud environments.
