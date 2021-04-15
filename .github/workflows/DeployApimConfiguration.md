# DeplopyApimConfiguration

A few parameters may be configured as environment variables in the yaml file.

## Parameters

| Parameter                  | Description |
| -------------------------- | ----------- |
| DESTINATIONAPINAME         | The name of the APIM instance that we want to send the configuration to, e.g. `myapim`|
| RESOURCEGROUP              | The resource group containing the APIM that we want to read, e.g. `apimRg` |
| FILEFOLDER                 | The folder on the repository that will contain the generated ARM Templates, e.g. `ApimTemplates` |
| BASEFILENAME               | The prefix of the generated files, e.g. `APIM` |
| SERVICEURL                 | The url's of the configured APIs (it should be a valid json string e.g. `"{'API1':'https://api1.com/api','AnotherApi':'https://api2.com/api',....,'LastApi':'https://lastapi.com/whatever'}"`|
| DEPLOYMENTMODE             | The ARM templates deployment mode. Should be set to `Incremental` (**unless you change the workflow, running it as `Complete` will delete your APIM instances** |
| DEPLOYMENTNAME             | The name of the deployment |
| DEPLOYGLOBALSERVICEPOLICY  | set to `${{ true }}` to include the Global Service Policy in the deployment, set to `${{ false }}` otherwise |
| DEPLOYAPIS                 | set to `${{ true }}` to include the APIs in the deployment, set to `${{ false }}` otherwise |
| DEPLOYAPIVERSIONSETS       | set to `${{ true }}` to include the API Version Sets in the deployment, set to `${{ false }}` otherwise |
| DEPLOYAUTHORIZATIONSERVERS | set to `${{ true }}` to include the Authorization Servers in the deployment, set to `${{ false }}` otherwise |
| DEPLOYLOGGERS              | set to `${{ true }}` to include the Loggers in the deployment, set to `${{ false }}` otherwise |
| DEPLOYPRODUCTS             | set to `${{ true }}` to include the Products in the deployment, set to `${{ false }}` otherwise |
| DEPLOYPRODUCTSAPIS         | set to `${{ true }}` to include the Products / API associations in the deployment, set to `${{ false }}` otherwise |
| DEPLOYAPITAGS              | set to `${{ true }}` to include the API Tags in the deployment, set to `${{ false }}` otherwise |
| DEPLOYNAMEDVALUES          | set to `${{ true }}` to include the Named Values in the deployment, set to `${{ false }}` otherwise |
| DEPLOYTAGS                 | set to `${{ true }}` to include the Tags in the deployment, set to `${{ false }}` otherwise |