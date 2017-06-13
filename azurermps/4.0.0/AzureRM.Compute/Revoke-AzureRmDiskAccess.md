---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Compute/Commands.Compute/help/Revoke-AzureRmDiskAccess.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Compute/Commands.Compute/help/Revoke-AzureRmDiskAccess.md
gitcommit: https://github.com/Azure/azure-powershell/blob/1e0dbd9ea7d5072fb8029e35f1a03f4023d1f52b
updated_at: 05/12/2017 03:05 AM
ms.date: 05/12/2017
ms.topic: reference
---

# Revoke-AzureRmDiskAccess

## SYNOPSIS
Revokes an access to a disk.

## SYNTAX

```
Revoke-AzureRmDiskAccess [-WhatIf] [-Confirm] [-ResourceGroupName] <String> [-DiskName] <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Revoke-AzureRmDiskAccess** cmdlet revokes an access to a disk.

## EXAMPLES

### Example 1
```
PS C:\> Revoke-AzureRmDiskAccess -ResourceGroupName 'ResourceGroup01' -DiskName 'Disk01'
```

Revoke the access to the disk named 'Disk01' in the resource group named 'ResourceGroup01'

## PARAMETERS

### -DiskName
Specifies the name of a disk.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
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
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs. The cmdlet is not run.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS
