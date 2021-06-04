# azure-templates
Azure ARM Templates for creating specific Azure Resources

## Table of Contents ##
- [Azure Templates Project](#azure-templates)
  * [Data Science Virtual Machine with Custom Script Extension](#data-science-virtual-machine-with-custom-script-extension)
  * [Cognitive Services](#cognitive-services)
  * [TODOs](#todos)

## Data Science Virtual Machine with Custom Script Extension ##

[template-dsvm-with-custom-script.json]

This creates a Windows 2019 DSVM and installs and configures IIS Webserver to run in it, via Custom Script Extension. In this case, the custom script is a PowerShell script [installWebServer.ps1].

Steps with an example - 

```sh
> az group create --name TRArmDSVM --location eastus
> az deployment group create --name TRArmDSVM --resource-group TRArmDSVM --template-file template-dsmv-with-custom-script.json
```

## Cognitive Services ##
...coming soon...

## TODOs ##
more templates

[//]: # (Comments in Markdown. See details here - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

[hashiLib]: <https://github.com/BetterCloud/vault-java-driver>
[MITL]: <https://en.wikipedia.org/wiki/MIT_License>

[template-dsvm-with-custom-script.json]: <https://github.com/tirtho/azure-templates/blob/master/template-dsmv-with-custom-script.json>
[installWebServer.ps1]: <https://github.com/tirtho/azure-templates/blob/master/installWebServer.ps1>
