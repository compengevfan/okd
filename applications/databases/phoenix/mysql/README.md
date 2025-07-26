##mysql

kubectl create namespace databases

kubectl apply -f /home/ladmin/git/k8s/applications/databases/phoenix/mysql/mysql-db-creds.yaml

kubectl apply -f /home/ladmin/git/k8s/applications/databases/phoenix/mysql/mysql-pvc-pv.yaml

kubectl apply -f /home/ladmin/git/k8s/applications/databases/phoenix/mysql/mysql-deployment.yaml

#kubectl apply -f /home/ladmin/git/k8s/applications/databases/phoenix/mysql/postgres-service.yaml

