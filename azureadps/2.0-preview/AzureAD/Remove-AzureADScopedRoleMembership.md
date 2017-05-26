---
external help file: Microsoft.Open.AzureADBeta.Graph.PowerShell.dll-Help.xml
ms.assetid: 937A2A6D-2DF5-43A5-8D2B-8555420254FB
online version:
schema: 2.0.0
updated_at: 04/25/2017 20:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-10/Azure%20AD%20Cmdlets/AzureAD/v2preview/Remove-AzureADScopedRoleMembership.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-10/Azure%20AD%20Cmdlets/AzureAD/v2preview/Remove-AzureADScopedRoleMembership.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/c5cc449ee6e2b805fc85a9e05130b06b10899f67
ms.topic: reference
ms.service: active-directory
---

# Remove-AzureADScopedRoleMembership

## SYNOPSIS
Removes a scoped role membership.

## SYNTAX

```
Remove-AzureADScopedRoleMembership -ObjectId <String> -ScopedRoleMembershipId <String> [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureADScopedRoleMembership** cmdlet removes a scoped role membership from Azure Active Directory (AD).

## EXAMPLES

## PARAMETERS

### -ObjectId
Specifies an object ID.

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
Specifies the ID of the scoped role membership to remove.

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

[Add-AzureADScopedRoleMembership](./Add-AzureADScopedRoleMembership.md)

[Get-AzureADScopedRoleMembership](./Get-AzureADScopedRoleMembership.md)
