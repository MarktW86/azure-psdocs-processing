---
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/preview/Azure%20AD%20Cmdlets/docs-conceptual/overview.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/preview/Azure%20AD%20Cmdlets/docs-conceptual/overview.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/a100da980eb7d179a5e13f962ccc29cc7bd90f9a
---
# Azure Active Directory PowerShell

Azure Active Directory PowerShell is the most commonly used user interface for IT Pros to manage their Azure Active Directory. These cmdlets cover a broad range of functionality that provide capabilities to retrieve data from the directory, create new objects in the directory or change existing objects and configure the directory and its features.

There are two PowerShell modules. The newer AzureAD V2 module implements the Graph API in PowerShell en provides a wide range of capabilities. The old MSOnline module can still be used for functionality that is not yet available in the AzureAD module.
If you are developing new PowerShell scripts with Azure AD cmdlets we advise you to use the newer [Azure Active Directory PowerShell V2 cmdlets](/module/azuread?view-azureadps-2.0). We will begin deprecating the older MSOnline module when all of the functionality of that module has been migrated to the newer AzureAD module.

Please refer to the below detailed description of the modules for a full list of cmdlets and functionality.


Module | Description
------ | -----------
[AzureAD](/powershell/module/azuread?view=azureadps-2.0) | Azure Active Directory PowerShell v2
[MSOnline](/powershell/module/msonline?view=azureadps-1.0)| Azure Active Directory PowerShell v1

