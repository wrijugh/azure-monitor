# Lab for 17 October 2023

## Pre-requisites
- Laptop, charger, plug point, table.
- Stable internet connection.
- Basic knowledge of Azure portal.
- Personal Microsoft Id (Outlook.com, Hotmail.com, Live.com preferred). To create new please use https://outlook.com. This will be used for giving access to Azure portal.
- Personal Github Id, this will be used for sharing the scripts and lab instruction. **We will use a private repo which is not available in public.** To create a new Github id, please use https://github.com/signup 

## Check the Azure Access
> Note: **Use private mode of browsing**
- To the personal email shared, an Azure access will be invited. You need to accept it from your mailbox. Check in the junk folder if it is not in inbox. 
- Once you follow the process, you will be able to login to Azure portal https://portal.azure.com/@wrijuhotmail.onmicrosoft.com 
- After you are able to login to the Azure portal, try creating a resource like Resource Group. 
- For running script use the Cloud Shell. Open Cloud Shell using https://shell.azure.com 


> Once you open the cloud shell, make sure your are using the right subscription. 

To check the current subscription use the below command

```bash
az account show
```

The output should look like, 

```json
{
  "environmentName": "AzureCloud", 
  "homeTenantId": "02f64eef-1937-431c-904f-021915601aac",
  "id": "7cc6dbb9-8bbe-4b9b-98a9-159a4d96e89b",
  "isDefault": true,
  "managedByTenants": [],
  "name": "Azure Pass - Sponsorship",
  "state": "Enabled",
  "tenantId": "02f64eef-1937-431c-904f-021915601aac",
  "user": {
    "cloudShellID": true,
    "name": "live.com#wriju@hotmail.com",
    "type": "user"
  }
}
```

If this is not showing the id as `7cc6dbb9-8bbe-4b9b-98a9-159a4d96e89b` and name as `Azure Pass - Sponsorship` then your are in the wrong subscription. Please logout and login again.

> In case you are have read access you can check it by running below command in Azure CLI. "Bash" mode of Cloud Shell.

```bash
az group list
```
---
[Next - Working with Azure Monitor](01-Lab-Implement_Monitoring.md)