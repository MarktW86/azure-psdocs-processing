---
external help file: Microsoft.Azure.Commands.Batch.dll-Help.xml
ms.assetid: AFDE5ECD-29AB-4C91-98BF-1B8C9C3BB079
online version:
schema: 2.0.0
updated_at: 03/11/2017 02:03 AM
ms.date: 03/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/staging/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.7.0/Get-AzureRmBatchAccountKeys.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/staging/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.7.0/Get-AzureRmBatchAccountKeys.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04f63f6e685743ace2c57eb157574e34e8610b1c
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: batch
---

# Get-AzureRmBatchAccountKeys

## SYNOPSIS
Gets the keys of a Batch account.

## SYNTAX

```
Get-AzureRmBatchAccountKeys [-AccountName] <String> [-ResourceGroupName <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmBatchAccountKeys** cmdlet gets the keys of an Azure Batch account in the current subscription.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -AccountName
Specifies the name of the account for which this cmdlet gets keys.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that contains the account for which this cmdlet gets keys.

```yaml
Type: String
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

## RELATED LINKS

[New-AzureRmBatchAccountKey](./New-AzureRmBatchAccountKey.md)

[Azure Batch Cmdlets](./AzureRM.Batch.md)


