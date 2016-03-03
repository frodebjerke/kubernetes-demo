Fireside Kubernetes - live demo cheat sheet
===

1. [console.cloud.google.com](console.cloud.google.com)
1. Show where to create a new cluster
1. `gcloud auth login`
1. `gcloud projects list`
1. `gcloud config set project lolcat-1236`
1. `gcloud container clusters get-credentials cow-cluster`
1. `kubectl get nodes`

## Create Pod
1. Show pod.yaml
1. `kubectl create -f k8s/pod.yaml`
1. `kubectl describe po hello-app`
1. `kubectl port-forward hello-app 8080:8080`

## Create Service for Pod
1. Show service.yaml
1. `kubectl create -f k8s/service.yaml`

## Create Replication Controller
1. Show rc.yaml
1. `kubectl create -f k8s/rc.yaml`
1. `k rolling-update hello-app --image=docker.io/frodetbj/fireside-demo-app:world`
