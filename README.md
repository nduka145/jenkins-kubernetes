# Installing jenkins on Kubernetes

## Steps to Install Jenkins on Kubernetes

### 1. Clone the repository  
Clone this Git repository to your local environment:

```bash
git clone https://github.com/nduka145/jenkins-kubernetes.git
cd jenkins-kubernetes
```

![image](https://github.com/user-attachments/assets/8955b4d1-3dbf-438d-ba66-678eb33c2b84)


### 2. Creating the Persistent volume, Persistent volume claim, deployment and service

```bash
kubectl apply -f pv.yml
kubectl apply -f pvc.yml
kubectl apply -f deployment.yml
kubectl apply -f service.yml

```
### Checking deployments and other status
```bash
kubectl get deployment
```bash
Output
![image](https://github.com/user-attachments/assets/b0fb1d56-73c8-4355-8036-a45ad9268766)
