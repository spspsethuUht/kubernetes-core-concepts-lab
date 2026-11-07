StatefulSet Lab
Objective
Deploy stateful workloads with stable identities.

Create
kubectl apply -f statefulset.yaml

Verify
Shell
kubectl get pods

Expected:

Plain Text
nginx-stateful-0
nginx-stateful-1
nginx-stateful-2
Delete Pod
Shell
kubectl delete pod nginx-stateful-1

Observe:

Shell
kubectl get pods

Pod recreated with same name.

Cleanup
Shell
kubectl delete -f .