---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Get-AzureRmApplicationGateway.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Get-AzureRmApplicationGateway.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
---

# Get-AzureRmApplicationGateway

## SYNOPSIS
Gets an application gateway.

## SYNTAX

```
Get-AzureRmApplicationGateway [-Name <String>] [-ResourceGroupName <String>] [<CommonParameters>]
```

## DESCRIPTION
The Get-AzureRmApplicationGateway cmdlet gets an application gateway.

## EXAMPLES

### --------------------------  Example 1: Get a specified application gateway  --------------------------
@{paragraph=PS C:\\\>}





```
PS C:\>$AppGw = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
```

This command gets the application gateway named ApplicationGateway01 that belongs to the resource group named ResourceGroup01 and stores it in the $AppGw variable.

### --------------------------  Example 2: Get a list of application gateways in a resource group  --------------------------
@{paragraph=PS C:\\\>}





```
PS C:\> $AppGwList = Get-AzureRmApplicationGateway -ResourceGroupName "ResourceGroup01"
```

This command gets a list of all the application gateways in the resource group named ResourceGroup01 and stores it in the $AppGwList variable.

### --------------------------  Example 3: Get a list of application gateways in a subscription  --------------------------
@{paragraph=PS C:\\\>}





```
PS C:\> $AppGwList = Get-AzureRmApplicationGateway
```

This command gets a list of all the application gateways in the subscription and stores it in the $AppGwList variable.

## PARAMETERS

### -Name
Specifies the name of the application gateway that this cmdlet gets.

```yaml
Type: String
Parameter Sets: (All)
Aliases: ResourceName

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that contains the application gateway.

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

### System.String

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGateway

### IEnumerable<Microsoft.Azure.Commands.Network.Models.PSApplicationGateway>

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, network, networking

## RELATED LINKS

[Stop-AzureRmApplicationGateway]()

