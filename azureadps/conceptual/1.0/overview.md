---
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/docs-conceptual/overview.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/docs-conceptual/overview.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/20594363af02af0e02d0c35738aa0298402344c3
---
# Azure Active Directory PowerShell

Azure Active Directory PowerShell (Azure AD) is a module IT Pros commonly use to manage their Azure Active Directory. The cmdlets in the Azure AD module enables you to retrieve data from the directory, create new objects in the directory, update existing objects, remove objects, as well as configure the directory and its features.

There are two vsersions of the Azure AD PowerShell modules. The earlier version, the MSOnline module, implemented core functionality and you can today still use this module. The newer AzureAD V2 module in an enhancement. The new module implements the Graph API in PowerShell. 

If you are developing new PowerShell scripts with Azure AD cmdlets we advise you to use the newer [Azure Active Directory PowerShell V2 cmdlets](/module/azuread?view-azureadps-2.0). We will begin deprecating the older MSOnline module when all of the functionality of that module has been migrated to the newer AzureAD module.

Please refer to the below detailed description of the modules for a full list of cmdlets and functionality.


Module | Description
------ | -----------
[AzureAD](/powershell/module/azuread?view=azureadps-2.0) | Azure Active Directory PowerShell v2
[MSOnline](/powershell/module/msonline?view=azureadps-1.0)| Azure Active Directory PowerShell v1

