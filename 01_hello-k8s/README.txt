# Deploy the app to Kubernetes using kubectl
kubectl apply -f k8s/deployment.yaml
kubectl get pods --selector app=demo

kubectl apply -f k8s/service.yaml
kubectl port-forward service/demo 9999:8888

http://localhost:9999/
