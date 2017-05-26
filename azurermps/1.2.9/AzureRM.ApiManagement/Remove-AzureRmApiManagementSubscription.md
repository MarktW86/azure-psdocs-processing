---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne052617/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Remove-AzureRmApiManagementSubscription.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne052617/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Remove-AzureRmApiManagementSubscription.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: api-Management
---

# Remove-AzureRmApiManagementSubscription

## SYNOPSIS
Deletes existing subscription.

## SYNTAX

```
Remove-AzureRmApiManagementSubscription -Context <PsApiManagementContext> -SubscriptionId <String> [-PassThru]
 [-Force] [<CommonParameters>]
```

## DESCRIPTION
Deletes existing subscription.

## EXAMPLES

### --------------------------  Example 1  --------------------------
@{paragraph=PS C:\\\>}





```
Remove-AzureRmApiManagementSubscription -Context $apimContext -SubscriptionId 0123456789 -Force
```

Delete existing subscription.

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
Identifier of existing subscription.
This parameter is required.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
If specified will write true in case operation succeeds.
This parameter is optional.
Default value is false.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Force
Forces delete operation (prevents confirmation dialog).
This parameter is optional.
Default value is false.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### bool

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, api, apimanagement, apimgmt, apism

## RELATED LINKS

