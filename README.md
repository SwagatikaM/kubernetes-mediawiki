# kubernetes-mediawiki
Installing Helm

  curl -L https://git.io/get_helm.sh | bash

  Helm init
  
Install Tiller on K8s cluster

  kubectl create - f tiller-sa.yaml

