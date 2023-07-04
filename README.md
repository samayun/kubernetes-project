<p align="center">
<img src="https://d1.awsstatic.com/PAC/kuberneteslogo.eabc6359f48c8e30b7a138c18177f3fd39338e05.png" />
</p>

#### STARTING

```
kubectl apply -f ./infra/k8s && kubectl apply -f ./infra/k8s-dev
```

#### Delete

```
kubectl delete -f ./infra/k8s && kubectl delete -f ./infra/k8s-dev
```

# How to Use Local Docker Images in Kubernetes

### 1

```bash

docker build -t samayunmc/client ./client && docker run samayunmc/client

eval $(minikube docker-env)


minikube image ls

```

### 2

```bash

docker build -t samayunmc/client ./client && docker run samayunmc/client

minikube image load samayunmc/client

minikube image ls

```

### samayun.com

```bash

echo "$(minikube ip) ticket-koi.com" | sudo tee -a /etc/hosts

cat /etc/hosts | tail -n 1


```
