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


#eclipse Maven

1️⃣ Check Maven Version
Steps

Press Windows + R

Type: cmd

Click OK

Type:

mvn -version


Press Enter

If you get 'mvn' not recognized → Maven not installed or PATH not added.

2️⃣ Create Maven Java Project (Using Eclipse)
Steps

Open Eclipse IDE

On top menu → click File

Click New

Click Project…

Expand Maven

Click Maven Project

Click Next

Check Create a simple project (skip archetype selection)

Click Next

Fill details:

Field	Value
Group Id	maven_java
Artifact Id	java_maven
Version	0.0.1-SNAPSHOT
Packaging	jar

Click Finish

3️⃣ Maven Java Project Structure (as shown in PDF)

In Project Explorer, you will see:

src/main/java  
src/test/java  
pom.xml  


No action needed — Eclipse creates it automatically.

4️⃣ Run the Java Program (Output in PDF)
Steps

Right-click src/main/java

Click New → Class

Enter:

Name: Demo     click:finish

Paste sample code:

public class Demo {
    public static void main(String[] args) {
        System.out.println("Maven Java Project");
    }
}        save with ctrl+s


Right-click on the file → Run As → Java Application     ---->>>MAVEN_JAVA
---------------Click New Repository (green button or “+” → “New repository”)                        
 Click Create Repository                                                                                                          Open your project folder in Terminal / PowerShell                                                              git init                                                                                                      git add .
 git commit -m "Initial Maven project commit"                                                                                                                              git remote add origin https://github.com/Navya-0408/my-maven-java-project.git                                                                                               git branch -M main
git push -u origin main
 DONE
