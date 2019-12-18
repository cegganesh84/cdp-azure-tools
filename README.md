# Cloudera CDP Tools for Microsoft Azure

A set of tools to help use Cloudera CDP with Microsoft Azure:

## Azure quickstart template

ARM template that deploys essential Azure resources for Cloudera CDP environment.


<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fcegganesh84%2Fcdp-azure-tools%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>

## Assumer identity role assignment

`
az deployment create --name assumerRoleAssignment --location westus2 --template-uri https://raw.githubusercontent.com/cegganesh84/cdp-azure-tools/master/assumerRoleAssignment.json --parameters '{"location": {"value": "westus2"},"assumerIdentityName": {"value": "cdppocAssumerIdentity"},"resourceGroupName": {"value": "cdppoc"}}'`