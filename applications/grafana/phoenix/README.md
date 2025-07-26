##mysql

kubectl create namespace grafana

kubectl apply -f /home/ladmin/git/k8s/applications/grafana/phoenix/mysql-db-creds.yaml

kubectl apply -f /home/ladmin/git/k8s/applications/grafana/phoenix/mysql-pvc-pv.yaml

kubectl apply -f /home/ladmin/git/k8s/applications/grafana/phoenix/mysql-deployment.yaml

kubectl apply -f /home/ladmin/git/k8s/applications/grafana/phoenix/mysql-service.yaml

##grafana

kubectl apply -f /home/ladmin/git/k8s/applications/grafana/phoenix/grafana-clusterip.yaml --namespace=grafana
#Create route