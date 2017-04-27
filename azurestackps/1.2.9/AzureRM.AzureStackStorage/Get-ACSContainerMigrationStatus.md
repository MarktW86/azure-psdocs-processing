---
external help file: Microsoft.AzureStack.AzureConsistentStorage.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/27/2017 13:04 PM
ms.date: 04/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/4.0.0/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackStorage/v0.10.6/Get-ACSContainerMigrationStatus.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/4.0.0/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackStorage/v0.10.6/Get-ACSContainerMigrationStatus.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/9a4c46f4a899f4d01966831d3cc84fd5672d8b5d
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# Get-ACSContainerMigrationStatus

## SYNOPSIS
{{Fill in the Synopsis}}

## SYNTAX

```
Get-ACSContainerMigrationStatus [-ResourceGroupName] <String> [-FarmName] <String> [-JobId] <String>
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
{{Fill FarmName Description}}

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
{{Fill ResourceGroupName Description}}

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
{{Fill SkipCertificateValidation Description}}

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
{{Fill SubscriptionId Description}}

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
{{Fill Token Description}}

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

