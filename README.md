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
### 3. Checking deployments and other status
```bash
kubectl get deployment
```
Output  
![image](https://github.com/user-attachments/assets/b0fb1d56-73c8-4355-8036-a45ad9268766)

```bash
kubectl get pod
```
Output  
![image](https://github.com/user-attachments/assets/4d6dc205-6b81-4e0e-a22b-1fce4766ae72)

```bash
kubectl get svc
```
Output  
![image](https://github.com/user-attachments/assets/7d9e4801-cdce-4381-a371-11489cf0cb10)

### 4. Assessing Jenkins
http://your_external-ip:3000

### 5. Getting Jenkins inital password
kubectl exec jenkins-667449857-65p75 -- cat /var/jenkins_home/secrets/initialAdminPassword

where jenkins-667449857-65p75 is your pod name as shown in the screenshot above. replace with your jenkins pod name





