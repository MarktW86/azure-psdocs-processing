---
external help file: Microsoft.Azure.Commands.Management.Storage.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/24/2017 22:05 PM
ms.date: 05/24/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Storage/v1.1.3/Get-AzureRmStorageAccount.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Storage/v1.1.3/Get-AzureRmStorageAccount.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/2d4a4fe807f8dce278c44747fc746934ed66d9fe
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: storage
---

# Get-AzureRmStorageAccount

## SYNOPSIS
Gets a storage account.

## SYNTAX

### AccountNameParameterSet
```
Get-AzureRmStorageAccount [-ResourceGroupName] <String> [-Name] <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### ResourceGroupParameterSet
```
Get-AzureRmStorageAccount [[-ResourceGroupName] <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmStorageAccount** cmdlet gets a specified storage account or all storage accounts within a resource group or the subscription.

## EXAMPLES

### Example 1: Get a specified storage account
```
Get-AzureRmStorageAccount -ResourceGroupName "rg1" -AccountName "mystorageaccount"
```

This example gets the storage account named "mystorageaccount" in the "rg1" resource group.

### Example 2: Get all storage accounts in a resource group
```
Get-AzureRmStorageAccount -ResourceGroupName "rg1"
```

This example gets all storage accounts in the "rg1" resource group.

### Example 3: Get all storage accounts in the subscription
```
Get-AzureRmStorageAccount
```

This example gets all storage accounts in the subscription.

## PARAMETERS

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

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
Specifies a variable that is used for storing an informational message.

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

### -Name
Specifies the name of the storage account to get.

```yaml
Type: String
Parameter Sets: AccountNameParameterSet
Aliases: StorageAccountName, AccountName

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that contains the storage account to get.

```yaml
Type: String
Parameter Sets: AccountNameParameterSet
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: ResourceGroupParameterSet
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### None

## NOTES

## RELATED LINKS

[New-AzureRmStorageAccount](./New-AzureRmStorageAccount.md)

[Remove-AzureRmStorageAccount](./Remove-AzureRmStorageAccount.md)

[Set-AzureRmStorageAccount](./Set-AzureRmStorageAccount.md)
