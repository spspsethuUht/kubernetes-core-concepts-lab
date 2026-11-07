NodePort Service Lab
Objective
Expose an application outside the cluster using a NodePort.

Create
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

Verify
Shell
kubectl get svc
 

Expected:

Plain Text
TYPE NodePort
PORT(S) 80:30080/TCP
Access Application
Shell
minikube service nodeport-service --url

Open browser.

Expected:

HTML
Welcome to nginx!
Cleanup
Shell
kubectl delete -f .

---

