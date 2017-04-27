---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/27/2017 22:04 PM
ms.date: 04/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Get-AzureRmApiManagementSubscription.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Get-AzureRmApiManagementSubscription.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a5140f27ab8f99c2992dc2ba0c9a1cd31941b109
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: api-Management
---

# Get-AzureRmApiManagementSubscription

## SYNOPSIS
Gets all or specific subscriptions.

## SYNTAX

### Get all subscriptions (Default)
```
Get-AzureRmApiManagementSubscription -Context <PsApiManagementContext>
```

### Get by subsctiption ID
```
Get-AzureRmApiManagementSubscription -Context <PsApiManagementContext> [-SubscriptionId <String>]
```

### Get by user ID
```
Get-AzureRmApiManagementSubscription -Context <PsApiManagementContext> [-UserId <String>]
```

### Get by product ID
```
Get-AzureRmApiManagementSubscription -Context <PsApiManagementContext> [-ProductId <String>]
```

## DESCRIPTION
Gets all or specific subscriptions.

## EXAMPLES

### --------------------------  Example 1  --------------------------
@{paragraph=PS C:\\\>}

```
Get-AzureRmApiManagementSubscription -Context $apimContext
```

Get all subscriptions.

### --------------------------  Example 2  --------------------------
@{paragraph=PS C:\\\>}

```
Get-AzureRmApiManagementSubscription -Context $apimContext -SubscriptionId 0123456789
```

Get subscription by Id.

### --------------------------  Example 3  --------------------------
@{paragraph=PS C:\\\>}

```
Get-AzureRmApiManagementSubscription -Context $apimContext -UserId 777
```

Get all users subscriptions.

### --------------------------  Example 4  --------------------------
@{paragraph=PS C:\\\>}

```
Get-AzureRmApiManagementSubscription -Context $apimContext -ProductId 999
```

Get all subscriptions for the product.

## PARAMETERS

### -Context
Instance of PsApiManagementContext.
This parameter is required.

```yaml
Type: PsApiManagementContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SubscriptionId
Subscription identifier.
If specified will try to find subscription by the identifier.
This parameter is optional.

```yaml
Type: String
Parameter Sets: Get by subsctiption ID
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UserId
User identifier.
If specified will try to find all subscriptions by the user identifier.
This parameter is optional.

```yaml
Type: String
Parameter Sets: Get by user ID
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ProductId
Product identifier.
If specified will try to find all subscriptions by the product identifier.
This parameter is optional.

```yaml
Type: String
Parameter Sets: Get by product ID
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### IList<Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementSubscription>

### Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementSubscription

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, api, apimanagement, apimgmt, apism

## RELATED LINKS

