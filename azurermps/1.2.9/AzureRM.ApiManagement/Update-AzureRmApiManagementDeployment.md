---
external help file: Microsoft.Azure.Commands.ApiManagement.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Update-AzureRmApiManagementDeployment.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Update-AzureRmApiManagementDeployment.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
---

# Update-AzureRmApiManagementDeployment

## SYNOPSIS
Updates deployment of an API Management Service.

## SYNTAX

### Specific API Management service (Default)
```
Update-AzureRmApiManagementDeployment -ResourceGroupName <String> -Name <String> -Location <String>
 -Sku <PsApiManagementSku> -Capacity <Int32> [-VirtualNetwork <PsApiManagementVirtualNetwork>]
 [-AdditionalRegions <System.Collections.Generic.IList`1[Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementRegion]>]
 [-PassThru] [<CommonParameters>]
```

### Update from PsApiManagement instance
```
Update-AzureRmApiManagementDeployment -ApiManagement <PsApiManagement> [-PassThru] [<CommonParameters>]
```

## DESCRIPTION
The Update-AzureRmApiManagementDeployment cmdlet updates current deployments of an API Management service.

## EXAMPLES

### Example 1: Update a deployment of an ApiManagement instance
```
PS C:\>Update-AzureRmApiManagementDeployment -ResourceGroupName "Contoso" -Name "ContosoApi" -Sku "Standard" -Capacity 3
```

This command updates deployment of an API Management instance to a three unit capacity standard.

### Example 2: Get an ApiManagement instance and rescale it
```
PS C:\>$ApiManagement = Get-AzureRmApiManagement -ResourceGroupName "Contoso" -Name "ContosoApi"
PS C:\> $ApiManagement.Sku = "Premium"
PS C:\> $ApiManagement.Capacity = 5
PS C:\> $ApiManagement.AddRegion("Central US", "Premium", 3)
PS C:\> Update-AzureRmApiManagementDeployment -ApiManagement $ApiManagement
```

This example gets an Api Management instance, scales it to five premium units and then adds an additional three units to the premium region.

## PARAMETERS

### -AdditionalRegions
Specifies additional deployment regions of Azure API Management.

```yaml
Type: System.Collections.Generic.IList`1[Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementRegion]
Parameter Sets: Specific API Management service
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApiManagement
Specifies the PsApiManagement instance to get deployment configuration from.
Use this parameter if the instance already has all the required changes.

```yaml
Type: PsApiManagement
Parameter Sets: Update from PsApiManagement instance
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Capacity
Specifies the SKU capacity of the master Azure API Management deployment region.

```yaml
Type: Int32
Parameter Sets: Specific API Management service
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Location
Specifies the location of the master API Management deployment region.

Valid values are:

-- North Central US
-- South Central US
-- Central US
-- West Europe
-- North Europe
-- West US
-- East US
-- East US 2
-- Japan East
-- Japan West
-- Brazil South
-- Southeast Asia
-- East Asia
-- Australia East
-- Australia Southeast

```yaml
Type: String
Parameter Sets: Specific API Management service
Aliases: 
Accepted values: North Central US, South Central US, Central US, West Europe, North Europe, West US, East US, East US 2, Japan East, Japan West, Brazil South, Southeast Asia, East Asia, Australia East, Australia Southeast

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of API Management that this cmdlet updates.

```yaml
Type: String
Parameter Sets: Specific API Management service
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
Specifies the name of resource group under which API Management exists.

```yaml
Type: String
Parameter Sets: Specific API Management service
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Sku
Specifies the tier of the master Azure API Management deployment region.

Valid values are:

-- Developer
-- Standard
-- Premium

```yaml
Type: PsApiManagementSku
Parameter Sets: Specific API Management service
Aliases: 
Accepted values: Developer, Standard, Premium

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VirtualNetwork
Specifies the Virtual Network configuration of the master Azure API Management deployment region.

```yaml
Type: PsApiManagementVirtualNetwork
Parameter Sets: Specific API Management service
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

[Get-AzureRmApiManagement]()

