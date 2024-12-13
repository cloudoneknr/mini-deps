create deployment.yaml file \
    kubectl apply -f deployment.yaml \
    kubectl get deployments \
Create nodeport service \
    kubectl apply -f service.yaml \
Test the deployment with port-foward \
    minikube service hello-minikube or kubectl port-forward service/hello-minikube 7080:8080 \
