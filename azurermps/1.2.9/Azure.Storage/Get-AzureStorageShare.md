---
external help file: Microsoft.WindowsAzure.Commands.Storage.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 03/27/2017 18:03 PM
ms.date: 03/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/Azure.Storage/v1.0.4.3/Get-AzureStorageShare.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/Azure.Storage/v1.0.4.3/Get-AzureStorageShare.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/9b79c0a37330eb2c43d3e7d31b5ab53f0da9554c
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: false
ms.service: storage
---

# Get-AzureStorageShare

## SYNOPSIS
{{Fill in the Synopsis}}

## SYNTAX

### MatchingPrefix (Default)
```
Get-AzureStorageShare [[-Prefix] <String>] [-Context <AzureStorageContext>] [-ServerTimeoutPerRequest <Int32>]
 [-ClientTimeoutPerRequest <Int32>] [-ConcurrentTaskCount <Int32>] [<CommonParameters>]
```

### Specific
```
Get-AzureStorageShare [-Name] <String> [-Context <AzureStorageContext>] [-ServerTimeoutPerRequest <Int32>]
 [-ClientTimeoutPerRequest <Int32>] [-ConcurrentTaskCount <Int32>] [<CommonParameters>]
```

### ShareName
```
Get-AzureStorageShare [-Context <AzureStorageContext>] [-ServerTimeoutPerRequest <Int32>]
 [-ClientTimeoutPerRequest <Int32>] [-ConcurrentTaskCount <Int32>] [<CommonParameters>]
```

## DESCRIPTION
{{Fill in the Description}}

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -ClientTimeoutPerRequest
The client side maximum execution time for each request in seconds.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConcurrentTaskCount
The total amount of concurrent async tasks.
The default value is 10.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Context
Azure Storage Context Object

```yaml
Type: AzureStorageContext
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Name
Name of the file share to be listed.

```yaml
Type: String
Parameter Sets: Specific
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Prefix
A prefix of the file shares to be listed.

```yaml
Type: String
Parameter Sets: MatchingPrefix
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServerTimeoutPerRequest
The server time out for each request in seconds.

```yaml
Type: Int32
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

### Microsoft.WindowsAzure.Commands.Common.Storage.AzureStorageContext

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

