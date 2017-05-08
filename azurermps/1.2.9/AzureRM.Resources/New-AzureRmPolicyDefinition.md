---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/02/2017 17:05 PM
ms.date: 05/02/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/DuncanmaMSFT-patch-1/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v1.0.4.3/New-AzureRmPolicyDefinition.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/DuncanmaMSFT-patch-1/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v1.0.4.3/New-AzureRmPolicyDefinition.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/fdff926f5dd35f9020f210f87b450464ba162edc
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-resource-manager
---

# New-AzureRmPolicyDefinition

## SYNOPSIS
Creates a new policy definition

## SYNTAX

```
New-AzureRmPolicyDefinition -Name <String> [-DisplayName <String>] [-Description <String>] -Policy <String>
 [-ApiVersion <String>] [-Pre] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
Creates a new policy definition

## EXAMPLES

### --------------------------  Create a new policy definition using policy file  --------------------------
@{paragraph=PS C:\\\>}



```
New-AzureRmPolicyDefinition -Name testDefinition -Policy C:\SamplePolicy.json
```

This will create a new policy definition 'testDefinition' with policy rule specified in C:\SamplePolicy.json file

### --------------------------  Create a new policy definition inline  --------------------------
@{paragraph=PS C:\\\>}



```
New-AzureRmPolicyDefinition -Name testDefinition -DisplayName "Test policy" -Policy "{""if"":{""source"":""action"",""equals"":""Microsoft.Compute/virtualMachines/write""},""then"":{""effect"":""deny""}}"
```

Creates a new policy definition 'testDefinition' with the specified policy

## PARAMETERS

### -ApiVersion
@{Text=}

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

### -Description
The description for policy definition

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DisplayName
The display name for policy definition

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
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

### -Name
The name for policy definition

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

### -Policy
The policy rule.
This can either be a path to a file name containing the policy rule, or the policy rule json as string

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

### -Pre
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

