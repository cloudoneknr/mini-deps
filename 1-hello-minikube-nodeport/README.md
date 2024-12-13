create deployment.yaml file \
    "\t"kubectl apply -f deployment.yaml \
    "\t"kubectl get deployments \
Create nodeport service \
    "\t"kubectl apply -f service.yaml \
Test the deployment with port-foward \
    "\t"minikube service hello-minikube or kubectl port-forward service/hello-minikube 7080:8080 \
