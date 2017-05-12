---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: 84FDB0F7-E6DE-4E1B-BD71-89535EDC6AA1
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Get-AzureRmEffectiveRouteTable.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Get-AzureRmEffectiveRouteTable.md
gitcommit: https://github.com/Azure/azure-powershell/blob/8810c0614b76be8d014616888a4ae7733a452af9
updated_at: 05/12/2017 03:05 AM
ms.date: 05/12/2017
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: virtual-network
---

# Get-AzureRmEffectiveRouteTable

## SYNOPSIS
Gets the effective route table of a network interface.

## SYNTAX

```
Get-AzureRmEffectiveRouteTable -NetworkInterfaceName <String> [-ResourceGroupName <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmEffectiveRouteTable** cmdlet returns the effective route table that is applied on a network interface.

## EXAMPLES

### Example 1: Get the effective route table on a network interface
```
PS C:\>Get-AzureRmEffectiveRouteTable -NetworkInterfaceName "MyNetworkInterface" -ResourceGroupName "MyResourceGroup"
```

This command gets the effective route table associated with network interface named MyNetworkInterface in the resource group named MyResourceGroup.

## PARAMETERS

### -NetworkInterfaceName
Specified the name of a network interface.

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

### -ResourceGroupName
Specifies the resource group of a network interface.

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

[Get-AzureRmEffectiveNetworkSecurityGroup](./Get-AzureRmEffectiveNetworkSecurityGroup.md)


