---
external help file: Microsoft.Azure.Commands.ApiManagement.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/27/2017 22:04 PM
ms.date: 04/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Set-AzureRmApiManagementVirtualNetworks.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Set-AzureRmApiManagementVirtualNetworks.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a5140f27ab8f99c2992dc2ba0c9a1cd31941b109
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: api-Management
---

# Set-AzureRmApiManagementVirtualNetworks

## SYNOPSIS
Sets the VPN configuration for an API Management Service.

## SYNTAX

```
Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName <String> -Name <String>
 [-VirtualNetworks <PsApiManagementVirtualNetwork[]>] [-PassThru]
```

## DESCRIPTION
The Set-AzureRmApiManagementVirtualNetworks cmdlet sets Virtual Network configuration for an API Management service.

## EXAMPLES

### Example 1: Set virtual networks for an API Management service
```
PS C:\>Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetworks $VirtualNetworks
```

This command sets virtual networks for an API Management service.

## PARAMETERS

### -Name
Specifies the name of an API Management service.

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

### -PassThru
Returns an object representing the item with which you are working.
By default, this cmdlet does not generate any output.

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

### -ResourceGroupName
Specifies the name of the resource group under which the API Management service exists.

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

### -VirtualNetworks
Specifies an array of virtual networks configurations.
Passing $null will remove the virtual network configuration.

```yaml
Type: PsApiManagementVirtualNetwork[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureRmApiManagementVirtualNetwork]()

