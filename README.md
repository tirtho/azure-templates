# azure-templates
Azure ARM Templates for creating specific Azure Resources

## Table of Contents ##
- [azure-templates](#azure-templates)
  * [Data Science Virtual Machine with Custom Script Extension](#data-science-virtual-machine-with-custom-script-extension)
  * [Cognitive Services](#cognitive-services)
  * [TODOs](#todos)
  * [License](#license)


## Data Science Virtual Machine with Custom Script Extension ##

template-dsvm-with-custom-script.json

This creates a Windows 2019 DSVM and installs and configures IIS Webserver to run in it, via Custom Script Extension.
Steps with an example - 

```sh
> az group create --name TRArmDSVM --location eastus
> az deployment group create --name TRArmDSVM --resource-group TRArmDSVM --template-file template-dsmv-with-custom-script.json
```

## Cognitive Services ##
...coming soon...

## TODOs ##
more templates

## License ##
