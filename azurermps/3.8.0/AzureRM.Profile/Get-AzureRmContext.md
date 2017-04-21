---
external help file: Microsoft.Azure.Commands.Profile.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/07/2017 09:04 AM
ms.date: 04/07/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/staging/azureps-cmdlets-docs/ResourceManager/AzureRM.Profile/v2.8.0/Get-AzureRmContext.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/staging/azureps-cmdlets-docs/ResourceManager/AzureRM.Profile/v2.8.0/Get-AzureRmContext.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/195dcb690a30a5f2c0ecd5606483862547ef544a
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: subscription
---

# Get-AzureRmContext

## SYNOPSIS
Gets the metadata used to authenticate Azure Resource Manager requests.

## SYNTAX

```
Get-AzureRmContext [<CommonParameters>]
```

## DESCRIPTION
The Get-AzureRmContext cmdlet gets the current metadata used to authenticate Azure Resource Manager requests.

This cmdlet gets the Active Directory account, Active Directory tenant, Azure subscription, and the targeted Azure environment.
Azure Resource Manager cmdlets use these settings by default when making Azure Resource Manager requests.

## EXAMPLES

### Example 1: Getting the current context
```
PS C:\> Add-AzureRmAccount
PS C:\> Get-AzureRmContext

Environment           : AzureCloud
Account               : test@outlook.com
TenantId              : xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
SubscriptionId        : yyyyyyyy-yyyy-yyyy-yyyy-yyyyyyyyyyyy
SubscriptionName      : Test Subscription
CurrentStorageAccount :
```

In this example we are logging into our account with an Azure subscription using Add-AzureRmAccount, and then we are getting the context of the current session by calling Get-AzureRmContext.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### PSAzureContext
This cmdlet returns the account, tenant, and subscription used by Azure Resource Manager cmdlets.

## NOTES

## RELATED LINKS

[Set-AzureRMContext]()

