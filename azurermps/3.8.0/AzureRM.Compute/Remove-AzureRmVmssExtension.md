---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
ms.assetid: 8C1C12AD-5130-42E7-99BB-B13900D7A712
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Compute/Commands.Compute/help/Remove-AzureRmVmssExtension.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Compute/Commands.Compute/help/Remove-AzureRmVmssExtension.md
gitcommit: https://github.com/Azure/azure-powershell/blob/1e0dbd9ea7d5072fb8029e35f1a03f4023d1f52b
updated_at: 04/28/2017 07:04 AM
ms.date: 04/28/2017
ms.topic: reference
---

# Remove-AzureRmVmssExtension

## SYNOPSIS
Removes an extension from the VMSS.

## SYNTAX

### NameParameterSet
```
Remove-AzureRmVmssExtension [-VirtualMachineScaleSet] <VirtualMachineScaleSet> [-Name] <String> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### IdParameterSet
```
Remove-AzureRmVmssExtension [-VirtualMachineScaleSet] <VirtualMachineScaleSet> -Id <String> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmVmssExtension** cmdlet removes an extension from the Virtual Machine Scale Set (VMSS).

## EXAMPLES

## PARAMETERS

### -Id
Specifies the ID of the extension that this cmdlet removes from the VMSS.

```yaml
Type: String
Parameter Sets: IdParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the extension that this cmdlet removes from the VMSS.

```yaml
Type: String
Parameter Sets: NameParameterSet
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VirtualMachineScaleSet
Specifies the VMSS from which to remove the extension from.

```yaml
Type: VirtualMachineScaleSet
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
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

## OUTPUTS

### This cmdlet does not generate any output.

## NOTES

## RELATED LINKS

[Add-AzureRmVmssExtension](./Add-AzureRmVmssExtension.md)
