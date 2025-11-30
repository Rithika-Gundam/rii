# kubernets

minikube start
docker login
minikube version
minikube status
kubectl create deployment myngnix --image=ngnix
kubectl get deployment
kubectl get pods
kubectl describe pods 
kubectl expose deployment myngnix --type-Nodeport --port=80 --target-port=80 --name=myngnix
kubectl get service myngnix
kubectl port-forward sevice/myngnix 3080:80
openbrowser and in url 127.0.0.1-3080
....
then open another powershell and 
minikube dashboard


# nagioss
docker pull jasonrivers/nagios:latest
docker images
docker run --name nagios4 -d -p 8888:80 jasonrivers/nagios:latest
docker start -ai nagios4


**#docker cli commands**
docker pull redis 
docker run --name my-redis -d redis 
docker ps 
docker exec -it my-redis redis-cli  
 docker stop my-redis
docker start my-redis 
docker rm my-redis  
docker rmi redis
docker run --name my-redis -d redis 
docker ps 
 docker logs my-redis 
docker network ls 
docker network create mynet 
docker run -d --name redis-server --network=mynet redis 
docker volume create mydata 
docker volume ls 
docker volume inspect mydata 
docker run -d --name my-reds -v mydata:/data redis 
docker rmi image-name 
docker pull redis
