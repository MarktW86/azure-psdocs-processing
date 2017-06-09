---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/4.1.0/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Remove-AzureRmApiManagementUserFromGroup.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/4.1.0/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Remove-AzureRmApiManagementUserFromGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
---

# Remove-AzureRmApiManagementUserFromGroup

## SYNOPSIS
Removes existing user from existing group.

## SYNTAX

```
Remove-AzureRmApiManagementUserFromGroup -Context <PsApiManagementContext> -GroupId <String> -UserId <String>
 [-PassThru] [<CommonParameters>]
```

## DESCRIPTION
Removes existing user from existing group.

## EXAMPLES

### --------------------------  Example 1  --------------------------
@{paragraph=PS C:\\\>}





```
Remove-AzureRmApiManagementUserFromGroup -Context $apimContext -GroupId 0001 -UserId 0123456789
```

Remove existing user from an existing group.

## PARAMETERS

### -Context
Instance of PsApiManagementContext.
This parameter is required.

```yaml
Type: PsApiManagementContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -GroupId
Identifier of existing group.
This parameter is required.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UserId
Identifier of existing user.
This parameter is required.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
If specified will write true in case operation succeeds.
This parameter is optional.
Default value is false.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, api, apimanagement, apimgmt, apism

## RELATED LINKS

