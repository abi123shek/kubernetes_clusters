#setting up minikube cluster

#first update system 
sudo apt-get update

#create folder minikube
mkdir minikube

#Wget is a command-line tool that makes it possible to download files from the internet directly to your active directory
 sudo apt install -y wget apt-transport-https
 
 #run minikube cmd for package installation
 curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube_latest_amd64.deb
sudo dpkg -i minikube_latest_amd64.deb

# now start minikube using cmd
 minikube start

#to see nodes
  kubectl get nodes

#to see all pods 
kubectl get po -A

#Halt the cluster
minikube stop

#Delete all of the minikube clusters
minikube delete
