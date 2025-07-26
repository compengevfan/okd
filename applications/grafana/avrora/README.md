##mysql

kubectl create namespace grafana

kubectl apply -f /home/ladmin/git/k8s/applications/grafana/avrora/mysql-db-creds-vault.yaml

kubectl apply -f /home/ladmin/git/k8s/applications/grafana/avrora/mysql-pvc-pv.yaml

kubectl apply -f /home/ladmin/git/k8s/applications/grafana/avrora/mysql-deployment.yaml

kubectl apply -f /home/ladmin/git/k8s/applications/grafana/avrora/mysql-service.yaml

##grafana

kubectl apply -f /home/ladmin/git/k8s/applications/grafana/avrora/grafana-clusterip.yaml --namespace=grafana
#Create route