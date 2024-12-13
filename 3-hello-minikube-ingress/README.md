create deployment.yaml file\
    &ensp;kubectl apply -f deployment.yaml\
    &ensp;kubectl get deployments\
Create loadbalncer service\
    &ensp;kubectl apply -f service.yaml\
Test the deployment with port-foward - start the tunnel to create a routable IP for the ‘balanced’ deployment:\
    &ensp;minikube tunnel\
    &ensp;kubectl get services hello-minikube (here you get routable public ip)\
    &ensp;Ex. http://127.0.0.1:8080/\
Test with ingress (add minikube ingress addon)\
    &ensp;minikube addons enable ingress\

