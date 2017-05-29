---
external help file: Microsoft.Open.MS.GraphBeta.PowerShell.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/25/2017 20:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/QuasarSE-doc-1/Azure%20AD%20Cmdlets/AzureAD/v2preview/Restore-AzureADMSDeletedDirectoryObject.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/QuasarSE-doc-1/Azure%20AD%20Cmdlets/AzureAD/v2preview/Restore-AzureADMSDeletedDirectoryObject.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/c5cc449ee6e2b805fc85a9e05130b06b10899f67
ms.topic: reference
ms.service: active-directory
---

# Restore-AzureADMSDeletedDirectoryObject

## SYNOPSIS
This cmdlet is used to restore a previously deleted object.

## SYNTAX

```
Restore-AzureADMSDeletedDirectoryObject -Id <String> [<CommonParameters>]
```

## DESCRIPTION
This cmdlet is used to restore a previously deleted object. Currently, only restoring Group and Application objects is supported. 
When a group or an application is deleted it is initially soft deleted and can be recovered during the first 30 days after deletion. After 30 days the deleted object is permanently deleted and can no longer be recovered. Note that only Unified Groups (a.k.a. Office 365 Groups) can be restored. Security groups cannot be restored.

## EXAMPLES

### Example 1
```
Restore-AzureADMSDeletedDirectoryObject -Id aa644285-eb75-4389-885e-7233f096984c
```

This example shows how to restore a deleted object with Id aa644285-eb75-4389-885e-7233f096984c 

## PARAMETERS

### -Id
The Id of the directory object to restore

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

