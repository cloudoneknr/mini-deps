create deployment.yaml file
    kubectl apply -f deployment.yaml
    kubectl get deployments
Create loadbalncer service
    kubectl apply -f service.yaml
Test the deployment with port-foward - start the tunnel to create a routable IP for the ‘balanced’ deployment:
    minikube tunnel
    kubectl get services hello-minikube (here you get routable public ip)
    Ex. http://127.0.0.1:8080/
Test with ingress (add minikube ingress addon)
    minikube addons enable ingress

