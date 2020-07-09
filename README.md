# azure-templates
Azure ARM Templates for creating specific Azure Resources

## Table of Contents ##
- [Azure Templates Project](#azure-templates)
  * [Data Science Virtual Machine with Custom Script Extension](#data-science-virtual-machine-with-custom-script-extension)
  * [Cognitive Services](#cognitive-services)
  * [TODOs](#todos)
  * [License](#license)


## Data Science Virtual Machine with Custom Script Extension ##

template-dsvm-with-custom-script.json

This creates a Windows 2019 DSVM and installs and configures IIS Webserver to run in it, via Custom Script Extension. In this case, the custom script is a PowerShell script installWebServer.ps1.

Steps with an example - 

```sh
> az group create --name TRArmDSVM --location eastus
> az deployment group create --name TRArmDSVM --resource-group TRArmDSVM --template-file template-dsmv-with-custom-script.json
```

## Cognitive Services ##
...coming soon...

## TODOs ##
more templates

License
----
[MIT License][MITL]


Copyright (c) 2020-2025 Tirthankar Barari

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


[//]: # (Comments in Markdown. See details here - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

[hashiLib]: <https://github.com/BetterCloud/vault-java-driver>
[MITL]: <https://en.wikipedia.org/wiki/MIT_License>

[template-dsvm-with-custom-script.json]: <https://github.com/tirtho/azure-templates/blob/master/template-dsmv-with-custom-script.json>
[installWebServer.ps1]: <https://github.com/tirtho/azure-templates/blob/master/installWebServer.ps1>
