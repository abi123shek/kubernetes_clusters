#here kind defines which type of file is creating

kind: Cluster
apiVersion: kind.x-k8s.io/v1alpha4


nodes:
- role: control-plane
  image: kindest/node:v1.16.4

- role: worker
  image: kindest/node:v1.16.4

- role: worker
  image: kindest/node:v1.16.4

- role: worker
  image: kindest/node:v1.16.4
  extraPortMappings:
  - containerPort: 80
    hostPort: 80
    protocol: TCP
  - containerPort: 443
    hostPort: 443
    protocol: TCP


#how to run after creating config_kind file
use cmd: kind create cluster --name=devcluster(your_cluster_name) --config=config.yml
