 
# How to setup two-tier application deployment on kubernetes cluster

First setup kubernetes kubeadm cluster

Use this repository to setup kubeadm [https://github.com/LondheShubham153/kubestarter/blob/main/kubeadm_installation.md](https://github.com/LondheShubham153/kubestarter/tree/main)

## Setup

1) First clone the code to your machine
```bash
  git clone https://github.com/LondheShubham153/two-tier-flask-app.git
   ```
2)Move to k8s directory
 ```bash
   cd two-tier-flask-app/k8s
   ```
3)Move to k8s directory
 ```bash
   cd two-tier-flask-app/k8s
   ```
4)Now, execute below commands one by one
```bash
   kubectl apply -f flask-deployment.yml
   ```
```bash
   kubectl apply -f flask-svc.yml
   ```
```bash
   kubectl apply -f mysql-deployment.yml
   ```
```bash
   kubectl apply -f mysql-svc.yml
   ```
```bash
   kubectl apply -f mysql-pv.yml
   ```
```bash
   kubectl apply -f mysql-pvc.yml
   ```
**To setup Helm in your server **
Use this repository to set-up helm [https://github.com/LondheShubham153/kubestarter/tree/main/HELM]

