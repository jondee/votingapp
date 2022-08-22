# votingapp
Voting-app

# PODS

kubectl create -f voting-app-pod.yml 
kubectl create -f redis-pod.yaml 
kubectl create -f postgres-pod.yaml
kubectl create -f worker-app-pod.yaml 
kubectl create -f result-app-pod.yml 

# Services 

kubectl create -f voting-app-service.yml 
kubeadm service voting-service --url
kubectl create -f redis-service.yml 
kubectl create -f postgres-service.yml 
kubectl create -f result-app-service.yml 
kubectl get svc
kubectl create -f 

# Deployment:
kubectl create -f voting-app-deployment.yml
kubectl create -f redis-deployment.yml
kubectl create -f postgres-deployment.yml
kubectl create -f  worker-app-deployment.yaml

kubectl create -f  result-app-deployment.yml

# Scale up
kubectl scale deployment voting-app-deploy --replicas = 3
