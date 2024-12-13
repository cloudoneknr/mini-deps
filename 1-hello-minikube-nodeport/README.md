create deployment.yaml file \
    \tkubectl apply -f deployment.yaml \
    \tkubectl get deployments \
Create nodeport service \
    \tkubectl apply -f service.yaml \
Test the deployment with port-foward \
    \tminikube service hello-minikube or kubectl port-forward service/hello-minikube 7080:8080 \
