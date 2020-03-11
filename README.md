# kubernetes-mediawiki
Installing Helm

  curl -L https://git.io/get_helm.sh | bash
  
Install Tiller on K8s cluster

  kubectl create - f tiller-sa.yaml

Initialize Helm with tiller account
  helm init --service-account=tiller --history-max 300
  
  kubectl get deployment tiller-deploy -n kube-system
  
  
   helm install --name mediawiki ./ helm install --name mediawiki . --set replicaCount=2
   helm inspect values .
   helm delete --purge mediawiki

