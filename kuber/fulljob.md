
kubectl apply -f app-deployment.yaml -n moviebot-ns

kubectl apply -f mongo-deployment.yaml -n moviebot-ns

--------
kubectl delete -f app-deployment.yaml

kubectl delete -f mongo-deployment.yaml

------
kubectl get pods -n moviebot-ns

kubectl logs -l app=moviebot -n moviebot-ns --tail=50


--------------------------
ps aux | grep moviebot.jar

ssh -i C:\Users\Redmi\.ssh\filonov.pem ubuntu@192.168.199.78 - basic

ssh -i ~/.ssh/filonov ubuntu@192.168.199.122 - openstack

ssh -i ~/.ssh/filonov ubuntu@84.201.157.148 - yandex