 # how to create multiple replicas while running
```kubectl scale deployment/my-deployment -n ownserver --replicas=10```
 # ensure that pod scale or not
 ```kubectl get pods -n ownserver```
 #whatif pod needs to be downgrade
 ```kubectl scale deployment/my-deployment -n ownserver --replicas=1```

*note here in 4th line deployment means your deployment.yml file and / my-deployment means your deployment metadata name 
