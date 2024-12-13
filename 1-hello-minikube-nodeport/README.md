create deployment.yaml file \
    &emsp;kubectl apply -f deployment.yaml \
    &emsp;kubectl get deployments \
Create nodeport service \
    &emsp;kubectl apply -f service.yaml \
Test the deployment with port-foward \
    &emsp;minikube service hello-minikube or kubectl port-forward service/hello-minikube 7080:8080
