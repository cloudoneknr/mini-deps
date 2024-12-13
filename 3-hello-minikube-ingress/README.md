create deployment.yaml file\
    "\t"kubectl apply -f deployment.yaml\
    "\t"kubectl get deployments\
Create loadbalncer service\
    "\t"kubectl apply -f service.yaml\
Test the deployment with port-foward - start the tunnel to create a routable IP for the ‘balanced’ deployment:\
    "\t"minikube tunnel\
    "\t"kubectl get services hello-minikube (here you get routable public ip)\
    "\t"Ex. http://127.0.0.1:8080/\
Test with ingress (add minikube ingress addon)\
    "\t"minikube addons enable ingress\

