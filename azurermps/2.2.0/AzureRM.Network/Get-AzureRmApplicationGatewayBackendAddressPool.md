---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Get-AzureRmApplicationGatewayBackendAddressPool.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Get-AzureRmApplicationGatewayBackendAddressPool.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
---

# Get-AzureRmApplicationGatewayBackendAddressPool

## SYNOPSIS
Gets a back-end address pool for an application gateway.

## SYNTAX

```
Get-AzureRmApplicationGatewayBackendAddressPool [-Name <String>] -ApplicationGateway <PSApplicationGateway>
 [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### --------------------------  Example 1: Get a specified backend server pool  --------------------------
@{paragraph=PS C:\\\>}





```
PS C:\> $AppGw = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $BackendPool = Get-AzureRmApplicationGatewayBackendAddressPool -Name "Pool01" -ApplicationGateway $AppGw
```

The first command gets the application gateway named ApplicationGateway01 in the resource group named ResourceGroup01 and stores it in the $AppGw variable.

### --------------------------  Example 2: Get a list of backend server pool  --------------------------
@{paragraph=PS C:\\\>}





```
PS C:\> $AppGw = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $BackendPools = Get-AzureRmApplicationGatewayBackendAddressPool -ApplicationGateway $AppGw
```

The first command gets the application gateway named ApplicationGateway01 in the resource group named ResourceGroup01 and stores it in the $AppGw variable.

## PARAMETERS

### -Name
Specifies the name of the back-end address pool that this cmdlet gets.

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

### -ApplicationGateway
The Get-AzureRmApplicationGatewayBackendAddressPool cmdlet gets a back-end address pool for an application gateway.

```yaml
Type: PSApplicationGateway
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayBackendAddressPool

### IEnumerable<Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayBackendAddressPool>

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, network, networking

## RELATED LINKS

[Add-AzureRmApplicationGatewayBackendAddressPool]()

[New-AzureRmApplicationGatewayBackendAddressPool]()

[Remove-AzureRmApplicationGatewayBackendAddressPool]()

[Set-AzureRmApplicationGatewayBackendAddressPool]()

