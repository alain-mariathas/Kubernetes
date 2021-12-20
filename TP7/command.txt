# kubectl create configmap appcolor --from-literal=color=red
kubectl create -f tp7-configmap.yml 
kubectl apply -f tp7-pod.yml
kubectl port-forward webapp  8080:8080 --address 0.0.0.0