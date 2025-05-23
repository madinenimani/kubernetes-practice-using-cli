eksctl create cluster \
  --name my-eks-cluster \
  --region us-east-1 \
  --nodegroup-name linux-nodes \
  --node-type t3.medium \
  --nodes 2 \
  --nodes-min 1 \
  --nodes-max 3 \
  --managed

# Check cluster status
eksctl get cluster --region us-east-1

# Check nodes
kubectl get nodes

# Check system pods
kubectl get pods -n kube-system





eksctl delete cluster --name my-eks-cluster --region us-east-1



