# arm-templates
This Repository contain useful ARM (Azure Resource Manager) Templates 


Resourse group has to be created at the scope of subsriptions. It would reque `az deployment` instead of `az deplyment grou`

```

az deployment validate --templatefile nestedtemplates/resourcegroup/resourcegroup.json --parameters @nestedtemplates/resourcegroup/params-resourcegroup.json


az deployment create --templatefile nestedtemplates/resourcegroup/resourcegroup.json --parameters @nestedtemplates/resourcegroup/params-resourcegroup.json


```


Validate ARM template with azure cli

`az group deployment validate --template-file nestedtemplates/logs/log-analytics.json --parameters @nestedtemplates/logs/log-analytics.params.json --resource-group my-rg | jq`

`az group deployment create --template-file nestedtemplates/logs/log-analytics.json --parameters @nestedtemplates/logs/log-analytics.params.json --resource-group my-rg | jq`


master json validate and create

```az group deployment validate --template-file master.json --resource-group my-rg | jq
az group deployment create --template-file master.json --resource-group my-rg | jq

