---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/02/2017 19:05 PM
ms.date: 05/02/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Set-AzureRMManagedSubscription.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Set-AzureRMManagedSubscription.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/64ea21b6f9d300bac04d2df45c463f94a5e389b4
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# Set-AzureRMManagedSubscription

## SYNOPSIS
Modifies the subscription of any tenant user.

## SYNTAX

```
Set-AzureRMManagedSubscription -Subscription <AdminSubscriptionDefinition>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-PipelineVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRMManagedSubscription** cmdlet modifies the subscription of any tenant user. The user must be logged in as a service administrator before issuing this cmdlet.

## EXAMPLES

### EXAMPLE 1: Change a property of a target subscription
```
$subscriptionToUpdate = Get-AzureRMManagedSubscription -TargetSubscriptionId "2fff214f-8589-4d25-b468-dc99320724bc"
$subscriptionToUpdate.OfferId = "Abc123"
Set-AzureRMManagedSubscription -Subscription $subscriptionToUpdate
```

This example modifies the **OfferId** property of the target subscription that has the subscription ID "2fff214f-8589-4d25-b468-dc99320724bc".
The first statement gets the subscription and stores the object in the $subscriptionToUpdate variable.
After the **OfferId** property is changed, the updated object is passed in the **Subscription** parameter of the **Set-AzureRMManagedSubscription** cmdlet.

## PARAMETERS

### -InformationAction
Specifies how this cmdlet responds to an information event.

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
Specifies a variable that is used for storing an informational message.

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
Specifies a variable that stores the value of the current pipeline element.

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

### -Subscription
Specifies an updated **AdminSubscriptionDefinition** object to be used for updating the existing subscription data.

```yaml
Type: AdminSubscriptionDefinition
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.AzureStack.Management.Models.SubscriptionDefinition

## OUTPUTS

### Microsoft.AzureStack.Management.Models.SubscriptionDefinition

## NOTES

## RELATED LINKS
