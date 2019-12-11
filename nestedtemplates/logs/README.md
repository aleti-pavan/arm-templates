
Steps:
-----
```
az login
az account set -s <subscription-id>

az group deployment create --resource-group <resource-group-name> --template-file .\log-analytics.azuredeploy.json --parameter .\log-analytics.parameters.json

```
