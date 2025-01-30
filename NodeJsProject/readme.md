# Frist you need to have a image
Step 1: clone github project or have docker image 
Step 2: create namespace.yml file and run it using cmd:kubectl apply -f namespace.yml
step 3: create deployment.yml file and run it using cmd:kubectl apply -f deployment.yml
step 4: create service.yml file and run it using cmd:kubectl apply -f service.yml
Step 5: ensue that all the configuration are running or not: use cmd: kubectl get all -n (your namespace)
step 6: use cmd to run your project and access from browser:kubectl port-forward service/notes-app-service -n notes-app 8000:8000 --address=0.0.0
