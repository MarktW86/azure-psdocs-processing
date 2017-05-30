---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/20/2017 04:04 AM
ms.date: 04/20/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-11/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADDomainNameReference.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-11/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADDomainNameReference.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/424c08eff259398d1aa2f26116c38cea5e911b45
ms.topic: reference
ms.service: active-directory
---

# Get-AzureADDomainNameReference

## SYNOPSIS
This cmdlet retrieves the objects that are referenced by a given domain name 

## SYNTAX

```
Get-AzureADDomainNameReference -Name <String> [<CommonParameters>]
```

## DESCRIPTION
This cmdlet retrieves the objects that are referenced by a given domain name 

## EXAMPLES

### Example 1
```
PS C:\WINDOWS\system32> Get-AzureADDomainNameReference -Name drumkit.onmicrosoft.com
```

This example shows how to retrieve the domain name reference objects for a domain that is specified through the -Name parameter

## PARAMETERS

### -Name
The name of the domain name for which the referenced objects are retrieved

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

### System.String

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

