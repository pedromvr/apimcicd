# GetApimConfiguration

A few parameters may be configured as environment variables in the yaml file

## Parameters

| Parameter          | Description |
| ------------------ | ----------- |
| SOURCEAPINAME      | The name of the APIM instance that we want to extract the configuration from, e.g. `mysourceapim` |
| RESOURCEGROUP      | The resource group containing the APIM that we want to read, e.g. `apimRg` |
| FILEFOLDER         | The folder on the repository that will contain the generated ARM Templates, e.g. `ApimTemplates` |
| BASEFILENAME       | The prefix of the generated files, e.g. `APIM` |
