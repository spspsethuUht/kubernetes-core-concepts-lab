LoadBalancer Service Lab
Objective
Expose services externally using a LoadBalancer.

Create
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml


Start Tunnel
Shell
minikube tunnel
Verify
Shell
kubectl get svc

Expected:

Plain Text
EXTERNAL-IP assigned
Test
Shell
curl http://EXTERNAL-IP