---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/25/2017 19:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71305/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Get-AzureRMManagedSubscription.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71305/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Get-AzureRMManagedSubscription.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/c4315559410058943d9b4bbae2b76e607f21de95
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# Get-AzureRMManagedSubscription

## SYNOPSIS
Gets details about the target subscription of the tenant user.

## SYNTAX

```
Get-AzureRMManagedSubscription [-TargetSubscriptionId <Guid>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-PipelineVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRMManagedSubscription** cmdlet gets details about the target subscription of the tenant user. This cmdlet is useful to a service administrator. You must be logged in as service administrator before issuing this command.

## EXAMPLES

### Example 1:
```
Get-AzureRMManagedSubscription -TargetSubscriptionId "2fff214f-8589-4d25-b468-dc99320724bc"
```

This command gets the target subscription details for the tenant user identified by the ID "2fff214f-8589-4d25-b468-dc99320724bc".

## PARAMETERS

### -InformationAction
Not Specified.

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
Not Specified.

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
Not Specified.

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
The target subscription ID of the tenant user.

```yaml
Type: Guid
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

### None

## OUTPUTS

### Microsoft.AzureStack.Management.Models.SubscriptionDefinition

## NOTES

## RELATED LINKS
