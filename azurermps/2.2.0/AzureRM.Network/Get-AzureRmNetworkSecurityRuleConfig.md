---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/27/2017 22:04 PM
ms.date: 04/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Get-AzureRmNetworkSecurityRuleConfig.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Get-AzureRmNetworkSecurityRuleConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a5140f27ab8f99c2992dc2ba0c9a1cd31941b109
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: virtual-network
---

# Get-AzureRmNetworkSecurityRuleConfig

## SYNOPSIS
Get a network security rule configuration for a network security group.

## SYNTAX

```
Get-AzureRmNetworkSecurityRuleConfig [-Name <String>] -NetworkSecurityGroup <PSNetworkSecurityGroup>
 [-DefaultRules] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## DESCRIPTION
The Get-AzureRmNetworkSecurityRuleConfig cmdlet gets a network security rule configuration for an Azure network security group.

## EXAMPLES

### --------------------------  Example 1  --------------------------
@{paragraph=PS C:\\\>}

```
Get-AzureRmNetworkSecurityGroup -Name  nsg1 -ResourceGroupName rg1 | Get-AzureRmNetworkSecurityRuleConfig -Name AllowInternetOutBound -DefaultRules
```

Retrieves the default rule named "AllowInternetOutBound" from Azure network security group named "nsg1" in resource group "rg1"

Name                     : AllowInternetOutBound
Id                       : /subscriptions/\<subscriptionId\>/resourceGroups/rg1/providers/Microsoft.N
                           etwork/networkSecurityGroups/nsg1/defaultSecurityRules/AllowInternetOutBound
Etag                     : W/"b4833539-3f97-4c90-ab00-8521d7f5ca35"
ProvisioningState        : Succeeded
Description              : Allow outbound traffic from all VMs to Internet
Protocol                 : *
SourcePortRange          : *
DestinationPortRange     : *
SourceAddressPrefix      : *
DestinationAddressPrefix : Internet
Access                   : Allow
Priority                 : 65001
Direction                : Outbound

### --------------------------  Example 2  --------------------------
@{paragraph=PS C:\\\>}

```
Get-AzureRmNetworkSecurityGroup -Name  nsg1 -ResourceGroupName rg1 | Get-AzureRmNetworkSecurityRuleConfig -Name "rdp-rule"
```

Retrieves user defined rule named "rdp-rule" from Azure network security group named "nsg1" in resource group "rg1"

Name                     : rdp-rule
Id                       : /subscriptions/\<subscriptionId\>/resourceGroups/rg1/providers/Microsoft.N
                           etwork/networkSecurityGroups/nsg1/securityRules/rdp-rule
Etag                     : W/"16f2b77c-1094-4bc5-91b0-07b81de13588"
ProvisioningState        : Succeeded
Description              : Allow RDP
Protocol                 : Tcp
SourcePortRange          : *
DestinationPortRange     : 3389
SourceAddressPrefix      : Internet
DestinationAddressPrefix : *
Access                   : Allow
Priority                 : 100
Direction                : Inbound

## PARAMETERS

### -Name
Specifies the name of the network security rule configuration to get.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkSecurityGroup
Specifies a NetworkSecurityGroup object that contains the network security rule configuration to get.

```yaml
Type: PSNetworkSecurityGroup
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DefaultRules
Indicates whether this cmdlet gets a user-created rule configuration or a default rule configuration.

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

## INPUTS

## OUTPUTS

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, network, networking

## RELATED LINKS

[Add-AzureRmNetworkSecurityRuleConfig]()

[New-AzureRmNetworkSecurityRuleConfig]()

[Remove-AzureRmNetworkSecurityRuleConfig]()

[Set-AzureRmNetworkSecurityRuleConfig]()

