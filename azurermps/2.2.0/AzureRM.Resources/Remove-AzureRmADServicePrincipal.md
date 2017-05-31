---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 22:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Remove-AzureRmADServicePrincipal.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Remove-AzureRmADServicePrincipal.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f7900661742fb361471ea2cb42574cb8d734fea4
ms.topic: reference
ms.service: azure-resource-manager
---

# Remove-AzureRmADServicePrincipal

## SYNOPSIS
Deletes the azure active directory service principal.

## SYNTAX

```
Remove-AzureRmADServicePrincipal -ObjectId <Guid> [-PassThru] [-Force] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Deletes the azure active directory service principal.

## EXAMPLES

### --------------------------  Delete AAD service principal.  --------------------------
@{paragraph=PS C:\\\>}



```
PS C:\> Remove-AzureRmADServicePrincipal -ObjectId 61b5d8ea-fdc6-40a2-8d5b-ad447c678d45
```

Deletes the given azure active directory service principal.

## PARAMETERS

### -ObjectId
The object id of the service principal to delete.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: PrincipalId

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
If specified, returns the deleted service principal.

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

### -WhatIf
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
{{Fill Force Description}}

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
Keywords: azure, azurerm, arm, resource, management, manager, resource, group, template, deployment

## RELATED LINKS

[New-AzureRmADServicePrincipal]()

[Get-AzureRmADServicePrincipal]()

[Set-AzureRmADServicePrincipal]()

[Remove-AzureRmADApplication]()

[Remove-AzureRmADAppCredential]()

