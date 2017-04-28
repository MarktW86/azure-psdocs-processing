---
external help file: Microsoft.AzureStack.AzureConsistentStorage.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/28/2017 21:04 PM
ms.date: 04/28/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71305/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackStorage/v0.10.6/Stop-ACSContainerMigration.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71305/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackStorage/v0.10.6/Stop-ACSContainerMigration.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/75431b1f2193df6595896df8a0c0bb66ae1d12ac
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# Stop-ACSContainerMigration

## SYNOPSIS
{{Fill in the Synopsis}}

## SYNTAX

```
Stop-ACSContainerMigration [-ResourceGroupName] <String> [-FarmName] <String> [-JobId] <String>
 [[-SubscriptionId] <String>] [[-Token] <String>] [[-AdminUri] <Uri>] [-SkipCertificateValidation]
 [<CommonParameters>]
```

## DESCRIPTION
{{Fill in the Description}}

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -AdminUri
Specifies the link, as a URI, to the service admin.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -FarmName


```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobId
{{Fill JobId Description}}

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 5
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName


```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SkipCertificateValidation


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

### -SubscriptionId


```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Token


```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String
System.Uri

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

