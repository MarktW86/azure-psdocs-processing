---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/20/2017 23:04 PM
ms.date: 04/20/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Remove-AzureRMTenantSubscription.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Remove-AzureRMTenantSubscription.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/d4f2539c40b2f09416fa3e1d384a0a1f0183fb5e
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# Remove-AzureRMTenantSubscription

## SYNOPSIS
The Remove-AzureRMTenantSubscription cmdlet removes the current logged in user's specified subscription.
There should not be any resources under the subscription to be removed

## SYNTAX

```
Remove-AzureRMTenantSubscription -TargetSubscriptionId <Guid> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-PipelineVariable <String>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### Example 1:
```
Remove-AzureRMTenantSubscription -TargetSubscriptionId $TenantSubscriptionId
```

Description

-----------

The example removes the specified tenant subscription id.

## PARAMETERS

### -InformationAction
Not Specified

The following values are permitted for this object type.

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa
Accepted values: SilentlyContinue, Stop, Continue, Inquire

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Not Specified

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PipelineVariable
Not Specified

```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetSubscriptionId
The current logged in user's Subscription Id to be removed

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.AzureOperationResponse

## NOTES

## RELATED LINKS

