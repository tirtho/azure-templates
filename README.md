# azure-templates
Azure ARM Templates for creating specific Azure Resources

template-dsvm-with-custom-script.json

This creates a Windows 2019 DSVM and installs and configures IIS Webserver to run in it, via Custom Script Extension.
Steps with an example - 
1. az group create --name TRArmDSVM --location eastus
2. az deployment group create --name TRArmDSVM --resource-group TRArmDSVM --template-file template-dsmv-with-custom-script.json
