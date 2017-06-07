---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Set-AzureRmApplicationGateway.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Set-AzureRmApplicationGateway.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
---

# Set-AzureRmApplicationGateway

## SYNOPSIS
Updates an application gateway.

## SYNTAX

```
Set-AzureRmApplicationGateway -ApplicationGateway <PSApplicationGateway> [<CommonParameters>]
```

## DESCRIPTION
The Set-AzureRmApplicationGateway cmdlet updates an Azure application gateway.

## EXAMPLES

### --------------------------  Example 1: Update an application gateway  --------------------------
@{paragraph=PS C:\\\>}



```
PS C:\> $UpdatedAppGw = Set-AzureRmApplicationGateway -ApplicationGateway $AppGw
```

This command updates the application gateway with settings in the $AppGw variable and stores the updated gateway in the $UpdatedAppGw variable.

## PARAMETERS

### -ApplicationGateway
Specifies an application gateway object representing the state to which the application gateway should be set.

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

## OUTPUTS

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, network, networking

## RELATED LINKS

[Start-AzureRmApplicationGateway]()

