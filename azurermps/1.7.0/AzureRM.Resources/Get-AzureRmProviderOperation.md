---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/27/2017 22:04 PM
ms.date: 04/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/Get-AzureRmProviderOperation.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/Get-AzureRmProviderOperation.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a5140f27ab8f99c2992dc2ba0c9a1cd31941b109
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-resource-manager
---

# Get-AzureRmProviderOperation

## SYNOPSIS
Gets the operations for an Azure resource provider that are securable using Azure RBAC.

## SYNTAX

```
Get-AzureRmProviderOperation [-OperationSearchString] <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## DESCRIPTION
The Get-AzureRmProviderOperation gets the operations exposed by Azure resource providers.
Operations can be composed to create custom roles in Azure RBAC.
The command takes as input an operation search string (with possible wildcard(*) character(s)) which determines the operations details to display.

Use Get-AzureRmProviderOperation * to get all operations for all Azure resource providers.

Use Get-AzureRmProviderOperation Microsoft.Compute/* to get all operations of Microsoft.Compute resource provider.

## EXAMPLES

### --------------------------  Get all actions for all providers  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\> Get-AzureRmProviderOperation *
```

### --------------------------  Get actions for a particular resource provider  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\> Get-AzureRmProviderOperation Microsoft.Insights/*
```

### --------------------------  Get all actions that can be performed on virtual machines  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\> Get-AzureRmProviderOperation */virtualMachines/*
```

## PARAMETERS

### -OperationSearchString
The operation search string (with possible wildcard (*) characters)

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InformationAction
@{Text=}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}

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

## INPUTS

## OUTPUTS

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, resource, group, template, deployment

## RELATED LINKS

