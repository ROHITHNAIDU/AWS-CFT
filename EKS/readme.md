1. create the Network stack using Network.yaml  
2. To create Amazon EKS cluster and Node group execute EKS.yaml cloudformation template.  
3. To connect to the EKS cluster created, we have to install Kubectl, eksctl, aws cli  
refer this link: https://docs.aws.amazon.com/eks/latest/userguide/getting-started.html   
4. once these softwares are installed, create Kubeconfig file, by executing this command  
"aws eks update-kubeconfig --region region-code --name my-cluster"  
5. then execute these commands  
kubectl get svc  
kubectl get nodes  
6. To create a deployment execute nginx-deployment.yaml. To create a service execute nginx-service.yaml  
7. To see the deployment, pods and service, execute these commands  
kubectl get svc  
kubectl get deployment  
kubectl get pods  
