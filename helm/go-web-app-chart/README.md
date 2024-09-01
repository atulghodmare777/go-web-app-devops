## How to start with helm
Install heml in the server
curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
chmod 700 get_helm.sh
./get_helm.sh
helm version
create folder called helm
Inside the helm run following command:
helm create go-web-app-chart
** Helm will create the configuration files for us such as templates charts chart.yaml values.yaml
update the files according to our requirement, in our case add deployment.yaml service.yaml ingress.yaml in the templates
and update the files accordingly as present in the folders in this repository
## After updating the files
```
heml install go-web-app ./go-web-app-chart
Our files has been deployed
```
## How to unistall helm
```
helm uninstall go-web-app
```
