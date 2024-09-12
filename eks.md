# important-commands-
1. Install AWS CLI:

```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
sudo apt install unzip -y
unzip awscliv2.zip
sudo ./aws/install
```

2. Install kubectl:

```bash
#!/bin/bash
sudo apt update
sudo apt install curl -y
sudo curl -LO "https://dl.k8s.io/release/v1.28.4/bin/linux/amd64/kubectl"
sudo chmod +x kubectl
sudo mv kubectl /usr/local/bin/
kubectl version --client
```
3. Install Helm:
```bash
sudo snap install helm --classic
```
4. Installing eksctl
```bash
curl --silent --location "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp
sudo mv /tmp/eksctl /usr/local/bin
eksctl version
```
5. The command you provided is used to update the kubeconfig file to allow communication with an Amazon EKS cluster.
   
```bash
aws eks update-kubeconfig --name dev-medium-eks-cluster --region us-east-1
```

