** setup

minikukbe destroy
minikube start

** run

kubectl apply -f deployment.yml
kubectl apply -f service.yml

# see what you are doing
minikube dashboard

# find port
kubectl get services
# find minikube vm IP
minikube status

** destroy

kubectl delete -f deployment.yml -f service.yml
