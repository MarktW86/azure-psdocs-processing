---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
ms.assetid: 29A39191-9E64-4983-8C89-B9A6C574E621
online version:
schema: 2.0.0
updated_at: 04/20/2017 04:04 AM
ms.date: 04/20/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/VinceSmith-patch-4/Azure%20AD%20Cmdlets/AzureAD/v2/New-AzureADDomain.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/VinceSmith-patch-4/Azure%20AD%20Cmdlets/AzureAD/v2/New-AzureADDomain.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/040cd8da6d7a72a69c1b4ba2f09d33e47e3b88c8
ms.topic: reference
ms.service: active-directory
---

# New-AzureADDomain

## SYNOPSIS
Creates a domain.

## SYNTAX

```
New-AzureADDomain [-IsDefault <Boolean>] -Name <String>
 [-SupportedServices <System.Collections.Generic.List`1[System.String]>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureADDomain** cmdlet creates a domain in Azure Active Directory (AD).

## EXAMPLES

## PARAMETERS

### -IsDefault
```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the domain.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SupportedServices
```yaml
Type: System.Collections.Generic.List`1[System.String]
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

[Confirm-AzureADDomain](./Confirm-AzureADDomain.md)

[Get-AzureADDomain](./Get-AzureADDomain.md)

[Remove-AzureADDomain](./Remove-AzureADDomain.md)

[Set-AzureADDomain](./Set-AzureADDomain.md)


