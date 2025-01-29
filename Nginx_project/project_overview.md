# Here in this project i am going to demonstrate from basic of all the thing like 

1.creating a kubernetes cluster (using kind cluster method)
2.creating namespace
3.creating pods
4. persistent volume
5 persistent volume claim
6 service (where we can view in browser)


for that all we need to do is to create yml file 

## frist of all create machine
you can create machine either in local or in cloud for now i am using aws instance to create this project

### update your machine 
must update your ubuntu machine using cmd: sudo apt-get update

#### install docker
use cmd: sudo apt-get install docker.io

Create the docker group if it does not exist:
use cmd:sudo groupadd docker

Add your user to the docker group:
use cmd:sudo usermod -aG docker $USER

Log in to the new docker group
use cmd:newgrp docker


##### install kubernetes using install.sh file 

##### config kind cluster using kind_config.yml file

##### create cluster using yml file  
how to run after creating kind_config file use cmd: kind create cluster --name=devcluster(your_cluster_name) --config=kind_config.yml

### create namespace
how to run after creating namespace file use cmd: kubectl apply -f ns (your name space)

#### create pod using yml file
how to run after creating pod.yml file use cmd: kubectl apply -f pod.yml ns (your namespace) 

## create deployment file
how to run after creating deployment.yml file use cmd: kubectl apply -f deployment.yml 

## create persistent volume

## create persistent volume claim





