---
external help file: Microsoft.Open.AzureADBeta.Graph.PowerShell.dll-Help.xml
ms.assetid: 142C8CA5-58AC-4D47-98D5-B3FB7E6A37C7
online version:
schema: 2.0.0
updated_at: 04/25/2017 20:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/rodejo5-10/Azure%20AD%20Cmdlets/AzureAD/v2preview/Get-AzureADScopedRoleMembership.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/rodejo5-10/Azure%20AD%20Cmdlets/AzureAD/v2preview/Get-AzureADScopedRoleMembership.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/c5cc449ee6e2b805fc85a9e05130b06b10899f67
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
ms.service: active-directory
---

# Get-AzureADScopedRoleMembership

## SYNOPSIS
Gets a scoped role membership from an administrative unit.

## SYNTAX

```
Get-AzureADScopedRoleMembership -ObjectId <String> [-ScopedRoleMembershipId <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureADScopedRoleMembership** cmdlet gets a scoped role membership from an administrative unit in Azure Active Directory (AD).

## EXAMPLES

## PARAMETERS

### -ObjectId
Specifies the ID of an object.
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

### -ScopedRoleMembershipId
Specifies the ID of a scoped role membership.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
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

[Add-AzureADScopedRoleMembership](./Add-AzureADScopedRoleMembership.md)

[Remove-AzureADScopedRoleMembership](./Remove-AzureADScopedRoleMembership.md)

