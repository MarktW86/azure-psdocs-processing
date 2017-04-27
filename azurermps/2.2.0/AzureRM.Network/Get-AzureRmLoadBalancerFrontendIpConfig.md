---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/27/2017 22:04 PM
ms.date: 04/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Get-AzureRmLoadBalancerFrontendIpConfig.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Get-AzureRmLoadBalancerFrontendIpConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a5140f27ab8f99c2992dc2ba0c9a1cd31941b109
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: virtual-network
---

# Get-AzureRmLoadBalancerFrontendIpConfig

## SYNOPSIS
Gets a front-end IP configuration in a load balancer.

## SYNTAX

```
Get-AzureRmLoadBalancerFrontendIpConfig [-Name <String>] -LoadBalancer <PSLoadBalancer>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## DESCRIPTION
The Get-AzureRmLoadBalancerFrontendIpConfig cmdlet gets a front-end IP configuration or a list of front-end IP configurations in a load balancer.

## EXAMPLES

### --------------------------  Example 1 Getting the frontend IP Configuration of an existing load balancer  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\> $slb = Get-AzureRmLoadBalancer -Name MyLoadBalancer -ResourceGroupName MyResourceGroup

PS C:\> Get-AzureRmLoadBalancerFrontendIpConfig -Name "MyFrontEnd" -LoadBalancer $slb
```

The first command gets the existing load balancer and stores it within the variable $slb.
The second command then gets the front end IP configuration associated with that load balancer.

Name                      : MyFrontEnd
Id                        : /subscriptions/xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx/resourceGroups/MyResourceGroup/providers/Microsoft.
                            Network/loadBalancers/MyLoadBalancer/frontendIPConfigurations/MyFrontEnd
Etag                      : W/"xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
ProvisioningState         : Succeeded
PrivateIpAddress          : 
PrivateIpAllocationMethod : Dynamic
Subnet                    : null
PublicIpAddress           : {
                              "Id": "/subscriptions/xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx/resourceGroups/MyResourceGroup/providers/M
                            icrosoft.Network/publicIPAddresses/MyPublicIP"
                            }
InboundNatRules           : \[
                              {
                                "Id": "/subscriptions/xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx/resourceGroups/MyResourceGroup/providers
                            /Microsoft.Network/loadBalancers/MyLoadBalancer/inboundNatRules/MyinboundNatRule1"
                              },
                              
                              }
                            \]
LoadBalancingRules        : \[
                              {
                                "Id": "/subscriptions/xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx/resourceGroups/MyResourceGroup/providers
                            /Microsoft.Network/loadBalancers/MyLoadBalancer/loadBalancingRules/MyLBruleName"
                              }
                            \]
InboundNatPools           : \[\]

## PARAMETERS

### -Name
Specifies the name of the load balancer that contains the front-end IP configuration to get.

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

### -LoadBalancer
Specifies the load balancer that is associated with the front-end IP configuration to get.

```yaml
Type: PSLoadBalancer
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

[Add-AzureRmLoadBalancerFrontendIpConfig]()

[New-AzureRmLoadBalancerFrontendIpConfig]()

[Remove-AzureRmLoadBalancerFrontendIpConfig]()

[Set-AzureRmLoadBalancerFrontendIpConfig]()

