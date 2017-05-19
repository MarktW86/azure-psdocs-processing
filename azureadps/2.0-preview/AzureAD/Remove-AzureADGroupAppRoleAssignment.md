---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
ms.assetid: F65ACCCF-86C4-4438-920F-289F5C69444E
online version:
schema: 2.0.0
updated_at: 04/25/2017 20:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-7/Azure%20AD%20Cmdlets/AzureAD/v2preview/Remove-AzureADGroupAppRoleAssignment.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-7/Azure%20AD%20Cmdlets/AzureAD/v2preview/Remove-AzureADGroupAppRoleAssignment.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/c5cc449ee6e2b805fc85a9e05130b06b10899f67
ms.topic: reference
ms.service: active-directory
---

# Remove-AzureADGroupAppRoleAssignment

## SYNOPSIS
Delete a group application role assignment.

## SYNTAX

```
Remove-AzureADGroupAppRoleAssignment -ObjectId <String> -AppRoleAssignmentId <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureADGroupAppRoleAssignment** cmdlet removes a group application role assignment from Azure Active Directory (AD).

## EXAMPLES

## PARAMETERS

### -AppRoleAssignmentId
Specifies the object ID of the group application role assignment.

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

### -ObjectId
Specifies the object ID of a group in Azure AD.

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

[Get-AzureADGroupAppRoleAssignment](./Get-AzureADGroupAppRoleAssignment.md)

[New-AzureADGroupAppRoleAssignment](./New-AzureADGroupAppRoleAssignment.md)
