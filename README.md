# arm-templates
This Repository contain useful ARM (Azure Resource Manager) Templates 


Validate ARM template with azure cli

`az group deployment validate --template-file nestedtemplates/logs/log-analytics.json --parameters @nestedtemplates/logs/log-analytics.params.json --resource-group my-rg | jq`

`az group deployment create --template-file nestedtemplates/logs/log-analytics.json --parameters @nestedtemplates/logs/log-analytics.params.json --resource-group my-rg | jq`


master json validate and create

```az group deployment validate --template-file master.json --resource-group my-rg | jq
az group deployment create --template-file master.json --resource-group my-rg | jq```

