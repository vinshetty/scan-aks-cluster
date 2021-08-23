# Scan AKS cluster
Scan AKS cluster using  **popeye** (https://github.com/derailed/popeye) tool  as a **Azure DevOps** Pipeline . 
Popeye is a utility that scans live Kubernetes cluster and reports potential issues with deployed resources and configurations. It sanitizes your cluster based on what's deployed and not what's sitting on disk. By scanning your cluster, it detects misconfigurations and helps you to ensure that best practices are in place, thus preventing future headaches. It aims at reducing the cognitive *over*load one faces when operating a Kubernetes cluster in the wild. Furthermore, if your cluster employs a metric-server, it reports potential resources over/under allocations and attempts to warn you should your cluster run out of capacity.
## Prerequisite
-	Resource Group Name
-	AKS cluster Name
-	K8s Namespace 
-	Azure service connection
-	Update below variables in attached Azure DevOps Pipeline
```
  **RG-NAME:** Resource Group of AKS cluster 
  **AKS-NAME:** AKS Cluster Name 
  **NAME-SPACE:** K8s Namespace
  **AZ-Connection:**  Azure Service Connection to connect azure cloud 
```
## OutPut/Result
