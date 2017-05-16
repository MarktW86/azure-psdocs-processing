---
external help file: Microsoft.WindowsAzure.Commands.Storage.dll-Help.xml
ms.assetid: E9500392-6BE1-46EC-9AF5-9234281025E6
online version:
schema: 2.0.0
updated_at: 05/12/2017 22:05 PM
ms.date: 05/12/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Storage/v3.0.0/New-AzureStorageQueue.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Storage/v3.0.0/New-AzureStorageQueue.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/3b96c1e0b28fc56dfbf6de55728d5478e0d02def
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: storage
---

# New-AzureStorageQueue

## SYNOPSIS
Creates a storage queue.

## SYNTAX

```
New-AzureStorageQueue [-Name] <String> [-Context <IStorageContext>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureStorageQueue** cmdlet creates a storage queue in Azure.

## EXAMPLES

### Example 1: Create an Azure storage queue
```
PS C:\>New-AzureStorageQueue -Name "queueabc"
```

This example creates a storage queue named queueabc.

### Example 2: Create multiple azure storage queues
```
PS C:\>"queue1 queue2 queue3".split() | New-AzureStorageQueue
```

This example creates multiple storage queues.
It uses the Split method of the .NET String class and then passes the names on the pipeline.

## PARAMETERS

### -Context
Specifies the Azure storage context.
You can create it by using the New-AzureStorageContext cmdlet.

```yaml
Type: IStorageContext
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Name
Specifies a name for the queue.

```yaml
Type: String
Parameter Sets: (All)
Aliases: N, Queue

Required: True
Position: 0
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

[Get-AzureStorageQueue](./Get-AzureStorageQueue.md)

[Remove-AzureStorageQueue](./Remove-AzureStorageQueue.md)


