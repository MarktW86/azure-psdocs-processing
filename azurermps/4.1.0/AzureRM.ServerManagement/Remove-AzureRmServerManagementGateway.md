---
external help file: Microsoft.Azure.Commands.ServerManagement.dll-Help.xml
ms.assetid: 41F8F851-6F9F-4DA4-8CE6-D8C9B7CF68D7
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/ServerManagement/Commands.ServerManagement/help/Remove-AzureRmServerManagementGateway.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/ServerManagement/Commands.ServerManagement/help/Remove-AzureRmServerManagementGateway.md
gitcommit: https://github.com/Azure/azure-powershell/blob/8810c0614b76be8d014616888a4ae7733a452af9
updated_at: 06/08/2017 20:06 PM
ms.date: 06/08/2017
ms.topic: reference
---

# Remove-AzureRmServerManagementGateway

## SYNOPSIS
Removes a Server Management gateway.

## SYNTAX

### ByName
```
Remove-AzureRmServerManagementGateway [-ResourceGroupName] <String> [-GatewayName] <String>
 [<CommonParameters>]
```

### ByObject
```
Remove-AzureRmServerManagementGateway [-Gateway] <Gateway> [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmServerManagementGateway** cmdlet removes an Azure Server Management gateway.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Gateway
Specifies the gateway that this cmdlet removes.

This parameter may be used instead of the *ResourceGroupName* and the *GatewayName* parameters.

```yaml
Type: Gateway
Parameter Sets: ByObject
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -GatewayName
Specifies the name of the gateway that this cmdlet removes.

```yaml
Type: String
Parameter Sets: ByName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group in that the gateway belongs to.

```yaml
Type: String
Parameter Sets: ByName
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
* All the nodes in the Gateway must be removed before using this cmdlet; otherwise this cmdlet will fail.

## RELATED LINKS

[Get-AzureRmServerManagementGateway](./Get-AzureRmServerManagementGateway.md)

[New-AzureRmServerManagementGateway](./New-AzureRmServerManagementGateway.md)


