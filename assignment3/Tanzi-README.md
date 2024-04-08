# ENSF 400 - Assignment 3 Procedure - Kubernetes
This is the step-by-step procedure for running this assignment

# Step One - Initializing
Initialize Minikube by running ```bash minikube start```.
This is to make the ```bash kubectl``` command use minikube.
Then run ```bash minikube addons enable ingress```.
This will allow Ingress to run.

# Step Two - Applying
Apply the changed files by running ```bash kubectl apply -f .```
Verify that it worked by running ```bash kubectl get pods``` and ```bash kubectl get services```.

# Step 3 - Running
Run the curl command by using ```bash curl http://$(minikube ip)/```
Running this multiple times should show the ratio of 7:3.
Your output should look similar to this:
![alt text](<Screenshot 2024-04-08 at 4.29.05 PM.png>)

# Step Four - Cleaning
Clear all pods by running ```bash kubectl delete -f .```
