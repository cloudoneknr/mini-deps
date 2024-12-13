create deployment.yaml file\
    \tkubectl apply -f deployment.yaml\
    \tkubectl get deployments\
Create loadbalncer service\
    \tkubectl apply -f service.yaml\
Test the deployment with port-foward - start the tunnel to create a routable IP for the ‘balanced’ deployment:\
    \tminikube tunnel\
    \tkubectl get services hello-minikube (here you get routable public ip)\
    \tEx. http://127.0.0.1:8080/\