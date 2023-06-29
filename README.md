INSTALL

$ kubectl create ns loki

$ helm template --name=promtail --namespace=loki --set loki.serviceName=loki-staging-headless -f values.yaml .| kubectl apply -f -
