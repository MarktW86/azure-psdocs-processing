---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/27/2017 22:04 PM
ms.date: 04/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/DuncanmaMSFT-patch-1/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Test-AzureRmPrivateIPAddressAvailability.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/DuncanmaMSFT-patch-1/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Test-AzureRmPrivateIPAddressAvailability.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a5140f27ab8f99c2992dc2ba0c9a1cd31941b109
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: virtual-network
---

# Test-AzureRmPrivateIPAddressAvailability

## SYNOPSIS
Test availability of a private IP address in a virtual network

## SYNTAX

### TestByResource
```
Test-AzureRmPrivateIPAddressAvailability -VirtualNetwork <PSVirtualNetwork> -IPAddress <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### TestByResourceId
```
Test-AzureRmPrivateIPAddressAvailability -ResourceGroupName <String> -VirtualNetworkName <String>
 -IPAddress <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## DESCRIPTION
The Test-AzureRmPrivateIPAddressAvailability cmdlet tests if a private IP address in a virtual network is available to use or not.
Return list of available private IP addresses if the requested private IP is taken.

## EXAMPLES

### --------------------------  Example 1  --------------------------
@{paragraph=PS C:\\\>}

```
Get-AzureRmvirtualNetwork -Name $vnetName -ResourceGroupName $rgname | Test-AzureRmPrivateIPAddressAvailability -IPAddress "10.0.1.10"
```

Test private IP address availability of a piped virtual network

### --------------------------  Example 2  --------------------------
@{paragraph=PS C:\\\>}

```
Test private IP address availability of a virtual network given its name and resource group name
```

Test private IP address availability of a virtual network given its name and resource group name

## PARAMETERS

### -VirtualNetwork
Specifies the virtual network to check availability for.

```yaml
Type: PSVirtualNetwork
Parameter Sets: TestByResource
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IPAddress
Specifies the IP address to check availability for.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
@{Text=}

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
@{Text=}

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

### -ResourceGroupName
Specifies the resource group name of the virtual network to check availability for.

```yaml
Type: String
Parameter Sets: TestByResourceId
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VirtualNetworkName
Specifies the virtual network name to check availability for.

```yaml
Type: String
Parameter Sets: TestByResourceId
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

