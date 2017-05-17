---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
ms.assetid: 04497A4E-E281-4FB5-98D5-102039F15692
online version:
schema: 2.0.0
updated_at: 04/20/2017 04:04 AM
ms.date: 04/20/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-5/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADDomain.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-5/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADDomain.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/040cd8da6d7a72a69c1b4ba2f09d33e47e3b88c8
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
ms.service: active-directory
---

# Get-AzureADDomain

## SYNOPSIS
Gets a domain.

## SYNTAX

### GetQuery (Default)
```
Get-AzureADDomain [<CommonParameters>]
```

### GetById
```
Get-AzureADDomain -Name <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureADDomain** cmdlet gets a domain in Azure Active Directory (AD).

## EXAMPLES

## PARAMETERS

### -Name
Specifies the name of a domain.
```yaml
Type: String
Parameter Sets: GetById
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Confirm-AzureADDomain](./Confirm-AzureADDomain.md)
[New-AzureADDomain](./New-AzureADDomain.md)
[Remove-AzureADDomain](./Remove-AzureADDomain.md)
[Set-AzureADDomain](./Set-AzureADDomain.md)


