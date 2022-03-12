# goFast
***
##Run step
$ docker build --tag docker-gs-ping .
$ docker image ls
$ docker image rm docker-gs-ping:v1.0
$ docker image tag docker-gs-ping:latest docker-gs-ping:v1.0
$ docker push belgarion111/docker-gs-ping:v1.0
$ docker run --publish 3000:3000 docker-gs-ping
$ docker login -u belgarion111

### Kubernetes
$ minikube start
$ kubectl apply -f .\deployment-update.yaml
$ kubectl get pods --> po
$ kubectl get deployments --> deploy
$ kubectl get svs
### On minikube no ingress no ClusterIp but only 
$ kubectl expose deployment gofast-deployment --type=LoadBalancer --port=3000
$ minikube tunnel
