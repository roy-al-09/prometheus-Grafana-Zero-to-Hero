# Install using Helm

## Add grafana helm-chart using helm repo

`helm repo add grafana https://grafana.github.io/helm-charts`

## Update helm repo

`helm repo update`

## Install grafana using the grafana helm-chart 

`helm install grafana grafana/grafana`

## Expose Grafana Service

`kubectl expose service grafana --type=NodePort --target-port=3000 --name=grafana-ext`
