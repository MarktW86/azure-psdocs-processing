---
external help file: Microsoft.Open.MS.GraphBeta.PowerShell.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/25/2017 20:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-9/Azure%20AD%20Cmdlets/AzureAD/v2preview/Remove-AzureADMSDeletedDirectoryObject.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-9/Azure%20AD%20Cmdlets/AzureAD/v2preview/Remove-AzureADMSDeletedDirectoryObject.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/c5cc449ee6e2b805fc85a9e05130b06b10899f67
ms.topic: reference
ms.service: active-directory
---

# Remove-AzureADMSDeletedDirectoryObject

## SYNOPSIS
This cmdlet is used to permanently delete a previously deleted directory object

## SYNTAX

```
Remove-AzureADMSDeletedDirectoryObject -Id <String> [<CommonParameters>]
```

## DESCRIPTION
This cmdlet is used to permanently delete a previously deleted directory object. When a directory object is permanently deleted it can no longer be restored.

## EXAMPLES

### Example 1
```
Remove-AzureADMSDeletedDirectoryObject -Id aa644285-eb75-4389-885e-7233f096984c
```

This example shows how to permanently delete a previously deleted directory object with Id = aa644285-eb75-4389-885e-7233f096984c

## PARAMETERS

### -Id
The Id of the directory object that is permanently deleted

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

