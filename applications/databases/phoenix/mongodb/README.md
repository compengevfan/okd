##mongodb

kubectl create namespace databases

kubectl apply -f /home/ladmin/git/k8s/applications/databases/phoenix/mongodb/mongodb-db-creds.yaml

kubectl apply -f /home/ladmin/git/k8s/applications/databases/phoenix/mongodb/mongodb-pvc-pv.yaml

kubectl apply -f /home/ladmin/git/k8s/applications/databases/phoenix/mongodb/mongodb-deployment.yaml

#kubectl apply -f /home/ladmin/git/k8s/applications/databases/phoenix/mongodb/postgres-service.yaml

