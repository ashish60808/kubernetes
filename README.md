# kubernetes
### Create the Configmap
kubectl create configmap prometheus-cm --from-file prometheus.yml -n <namespace>
  
### Create the deployment
kubectl apply -f prometheus-deployment.yml  -n <namespace>
  
### Create the service
kubectl apply -f prometheus-service.yml  -n <namespace>
  
### Create the Ingress
kubectl apply -f prometheus-ingress.yml  -n <namespace>
