
kubectl apply -f app-deployment.yaml -n moviebot-ns
kubectl apply -f mongo-deployment.yaml -n moviebot-ns

kubectl delete -f app-deployment.yaml
kubectl delete -f mongo-deployment.yaml

kubectl get pods -n moviebot-ns
kubectl logs -l app=moviebot -n moviebot-ns --tail=50