---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: 2A3B7343-9AA0-4505-AEDE-31C0C5B98694
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Set-AzureRmExpressRouteCircuit.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Set-AzureRmExpressRouteCircuit.md
gitcommit: https://github.com/Azure/azure-powershell/blob/39673ed92d863c7fba7fbbdb0d919d03c552b71b
updated_at: 05/12/2017 03:05 AM
ms.date: 05/12/2017
ms.topic: reference
---

# Set-AzureRmExpressRouteCircuit

## SYNOPSIS
Modifies an ExpressRoute circuit.

## SYNTAX

```
Set-AzureRmExpressRouteCircuit -ExpressRouteCircuit <PSExpressRouteCircuit> [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmExpressRouteCircuit** cmdlet saves the modified ExpressRoute circuit to Azure.

## EXAMPLES

### Example 1: Change the ServiceKey of an ExpressRoute circuit
```
$ckt = Get-AzureRmExpressRouteCircuit -Name $CircuitName -ResourceGroupName $rg
$ckt.ServiceKey = '64ce99dd-ee70-4e74-b6b8-91c6307433a0'
Set-AzureRmExpressRouteCircuit -ExpressRouteCircuit $ckt
```

## PARAMETERS

### -ExpressRouteCircuit
Specifies the **ExpressRouteCircuit** object that this cmdlet modifies.

```yaml
Type: PSExpressRouteCircuit
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

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmExpressRouteCircuit](./Get-AzureRmExpressRouteCircuit.md)

[Move-AzureRmExpressRouteCircuit](./Move-AzureRmExpressRouteCircuit.md)

[New-AzureRmExpressRouteCircuit](./New-AzureRmExpressRouteCircuit.md)

[Remove-AzureRmExpressRouteCircuit](./Remove-AzureRmExpressRouteCircuit.md)
