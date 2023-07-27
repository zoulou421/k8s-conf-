# MongoDb kubernetes configMap components
##learn how to configure mongo db with secret in configMap k8s component
start by creating secret file file first:
echo -n 'username' | base64
echo -n 'password' | base64

kubectl apply -f mongo_secret.yaml
kubectl get secret

put secret in deployment:
kubectl apply -f mongo_deploymnt.yaml




