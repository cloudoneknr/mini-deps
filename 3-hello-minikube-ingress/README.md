create deployment.yaml file\
    &emsp;kubectl apply -f deployment.yaml\
    &emsp;kubectl get deployments\
Create loadbalncer service\
    &emsp;kubectl apply -f service.yaml\
Test the deployment with port-foward - start the tunnel to create a routable IP for the ‘balanced’ deployment:\
    &emsp;minikube tunnel\
    &emsp;kubectl get services hello-minikube (here you get routable public ip)\
    &emsp;Ex. http://127.0.0.1:8080/\
Test with ingress (add minikube ingress addon)\
    &emsp;minikube addons enable ingress\

