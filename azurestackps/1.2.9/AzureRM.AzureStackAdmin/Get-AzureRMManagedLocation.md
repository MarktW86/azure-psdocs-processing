---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/02/2017 19:05 PM
ms.date: 05/02/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Get-AzureRMManagedLocation.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Get-AzureRMManagedLocation.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/64ea21b6f9d300bac04d2df45c463f94a5e389b4
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# Get-AzureRMManagedLocation

## SYNOPSIS
Gets the details about a location managed by the Azure stack resource manager.

## SYNTAX

```
Get-AzureRMManagedLocation [-Name <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-PipelineVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmMangedLocation** cmdlet gets the details about a location managed by the Azure stack resource manager.

## EXAMPLES

### Example 1: Get details about the location having the specified name
```
Get-AzureRMManagedLocation -Name "Chicago"
```

This example gets the details of the location named "Chicago".

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

### -Name
Specifies the name of the location.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### Microsoft.AzureStack.Management.Models.Location

## NOTES

## RELATED LINKS
