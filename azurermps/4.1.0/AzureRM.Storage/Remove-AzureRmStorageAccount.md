---
external help file: Microsoft.Azure.Commands.Management.Storage.dll-Help.xml
ms.assetid: 006B4341-274C-4929-86EE-2E107BA9E485
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Storage/Commands.Management.Storage/help/Remove-AzureRmStorageAccount.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Storage/Commands.Management.Storage/help/Remove-AzureRmStorageAccount.md
gitcommit: https://github.com/Azure/azure-powershell/blob/8810c0614b76be8d014616888a4ae7733a452af9
updated_at: 06/08/2017 20:06 PM
ms.date: 06/08/2017
ms.topic: reference
---

# Remove-AzureRmStorageAccount

## SYNOPSIS
Removes a Storage account from Azure.

## SYNTAX

```
Remove-AzureRmStorageAccount [-ResourceGroupName] <String> [-Name] <String> [-Force] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmStorageAccount** cmdlet removes a Storage account from Azure.

## EXAMPLES

### Example 1: Remove a Storage account
```
PS C:\>Remove-AzureRmStorageAccount -ResourceGroupName "RG01" -AccountName "MyStorageAccount"
```

This command removes the specified Storage account.

## PARAMETERS

### -Force
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

### -Name
Specifies the name of the Storage account to remove.

```yaml
Type: String
Parameter Sets: (All)
Aliases: StorageAccountName, AccountName

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that contains the Storage account to remove.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmStorageAccount](./Get-AzureRmStorageAccount.md)

[New-AzureRmStorageAccount](./New-AzureRmStorageAccount.md)

[Set-AzureRmStorageAccount](./Set-AzureRmStorageAccount.md)


