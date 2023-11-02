# Assignment_kubernetes
1. To create a docker image we have to make Dockerfile <br>
   and build it using following command<br>
   ```sudo docker build -t anirudhabidave/kube-assignment .```<br>
2. To push the image on docker hub first we have to login <br>
   ```sudo docker login```<br>
   and put your username and password of docker hub<br>
   To push the image the command is<br>
   ```sudo docker push anirudhabidave/kube-assignment```<br>
3. To deploy the java app on kubernetes we have two ways<br>
    I. By creating pod.yaml file and service.yaml file<br>
       To create a pod <br>
       ```kubectl create -f mypod.yaml```<br>
       To create a sirvice.yaml file <br>
       ```kubectl create -f service-definition.yaml```<br>
       To get the link to access the web app<br>
       ```minikube service myapp-service --url```<br>
   II. By creating deployment.yaml and service.yaml files<br>
       To create a deployment.yaml file<br>
       ```kubectl create -f deployment.yaml```<br>
       To create a service.yaml<br>
       ```kubectl create -f service-definition.yaml```<br>
       To get the link for accessing the web app <br>
       ```minikube service myapp-service --url```<br>
