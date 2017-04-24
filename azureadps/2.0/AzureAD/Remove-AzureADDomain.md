---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
ms.assetid: CAD38E2B-DC2D-440F-A51F-1CF9060FF62A
online version:
schema: 2.0.0
updated_at: 04/24/2017 22:04 PM
ms.date: 04/24/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2-preview/Remove-AzureADDomain.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2-preview/Remove-AzureADDomain.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/e8fee4f7b154d51007aafbde860e493d3e63a77e
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
ms.service: active-directory
---

# Remove-AzureADDomain

## SYNOPSIS
Removes a domain.

## SYNTAX

```
Remove-AzureADDomain -Name <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureADDomain** cmdlet removes a domain from Azure Active Directory (AD).

## EXAMPLES

## PARAMETERS

### -InformationAction
Specifies how this cmdlet responds to an information event. The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

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
Specifies an information variable.

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
Specifies the name of the domain to remove.
```yaml
Type: String
Parameter Sets: (All)
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

[Get-AzureADDomain](./Get-AzureADDomain.md)

[New-AzureADDomain](./New-AzureADDomain.md)

[Set-AzureADDomain](./Set-AzureADDomain.md)
