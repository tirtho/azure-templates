# azure-templates
Azure ARM Templates for creating specific Azure Resources

## Table of Contents ##
- [Azure Templates Project](#azure-templates)
  * [Data Science Virtual Machine with Custom Script Extension](#data-science-virtual-machine-with-custom-script-extension)
  * [Azure Function App (python)](#azure-python-function-app)
  * [TODOs](#todos)

## Data Science Virtual Machine with Custom Script Extension ##

[template-dsvm-with-custom-script.json]

This creates a Windows 2019 DSVM and installs and configures IIS Webserver to run in it, via Custom Script Extension. In this case, the custom script is a PowerShell script [installWebServer.ps1].

Steps with an example - 

```sh
> az group create --name TRArmDSVM --location eastus
> az deployment group create --name TRArmDSVM --resource-group TRArmDSVM --template-file template-dsmv-with-custom-script.json
```

## Azure Python Function App ##

[template-azure-python-function.json]

This creates a Linux Python Function App. 

Steps to deploy is below. Running the deployment script below will ask you for your Azure Subscription id. 

```sh
> az group create --name TRPythonFunc --location eastus
> az deployment group create --resource-group TRPythonFunc --template-file template-azure-python-function.json
```
Note: You can put your subscription id in a parameters.json file as below. Then in the 'az deployment command above, pass --parameters parameters.json.

```
{
    "$schema": "https://schema.management.azure.com/schemas/2015-01-01/deploymentParameters.json#",
    "contentVersion": "1.0.0.0",
    "parameters": {
        "subscriptionId": {
            "value": "<your subscription id>"
        }
    }
}
```

## TODOs ##
more templates

[//]: # (Comments in Markdown. See details here - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

[hashiLib]: <https://github.com/BetterCloud/vault-java-driver>
[MITL]: <https://en.wikipedia.org/wiki/MIT_License>

[template-azure-python-function.json]: <https://github.com/tirtho/azure-templates/blob/master/template-azure-python-function.json>
[template-dsvm-with-custom-script.json]: <https://github.com/tirtho/azure-templates/blob/master/template-dsmv-with-custom-script.json>
[installWebServer.ps1]: <https://github.com/tirtho/azure-templates/blob/master/installWebServer.ps1>
