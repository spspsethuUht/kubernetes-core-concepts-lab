# ClusterIP Notes

## What is ClusterIP?

ClusterIP is the default Kubernetes Service type.

It exposes an application only within the Kubernetes cluster.

External users cannot access a ClusterIP service directly.

## Typical Use Cases

- Frontend communicating with Backend
- Backend communicating with Database
- Internal Microservices Communication

## Traffic Flow

Client Pod

↓

ClusterIP Service

↓

Application Pod

## Advantages

- Secure
- Internal Access Only
- No External Exposure Required

## Key Takeaway

Use ClusterIP whenever applications need communication only within the cluster.
