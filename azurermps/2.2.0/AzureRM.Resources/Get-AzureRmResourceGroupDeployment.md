---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
ms.assetid: 886F29CC-4A82-403A-94FB-6D35258A3050
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Get-AzureRmResourceGroupDeployment.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Get-AzureRmResourceGroupDeployment.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
---

# Get-AzureRmResourceGroupDeployment

## SYNOPSIS
Gets the deployments in a resource group.

## SYNTAX

### The deployment name parameter set. (Default)
```
Get-AzureRmResourceGroupDeployment [-ResourceGroupName] <String> [[-Name] <String>] [-ApiVersion <String>]
 [-Pre] [<CommonParameters>]
```

### The deployment Id parameter set.
```
Get-AzureRmResourceGroupDeployment -Id <String> [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmResourceGroupDeployment** cmdlet gets the deployments in an Azure resource group.
Specify the *Name* or *Id* parameter to filter the results.
By default, **Get-AzureRmResourceGroupDeployment** gets all deployments for a specified resource group.

An Azure resource is a user-managed Azure entity, such as a database server, database, or web site.
An Azure resource group is a collection of Azure resources that are deployed as a unit.

A deployment is the operation that makes the resources in the resource group available for use.
For more information about Azure resources and Azure resource groups, see the **New-AzureRmResourceGroup** cmdlet.

You can use this cmdlet for tracking.
For debugging, use this cmdlet with the **Get-AzureRmLog** cmdlet.

## EXAMPLES

### Example 1: Get all deployments for a resource group
```
PS C:\> Get-AzureRmResourceGroupDeployment -ResourceGroupName "ContosoLabsRG"
```

This command gets all deployments for the ContosoLabsRG resource group.
The output shows a deployment for a WordPress blog that used a gallery template.

### Example 2: Get a deployment by name
```
PS C:\> Get-AzureRmResourceGroupDeployment -ResourceGroupName "ContosoLabsRG" -Name "DeployWebsite01"
```

This command gets the DeployWebsite01 deployment of the ContosoLabsRG resource group.
You can assign a name to a deployment when you create it by using the **New-AzureRmResourceGroup** or **New-AzureRmResourceGroupDeployment** cmdlets.
If you do not assign a name, the cmdlets provide a default name based on the template that is used to create the deployment.

### Example 3: Get the deployments of all resource groups
```
PS C:\> Get-AzureRmResourceGroup | Get-AzureRmResourceGroupDeployment | Format-Table ResourceGroupName, DeploymentName, ProvisioningState
```

This command gets all resource groups in your subscription by using the **Get-AzureRMResourceGroup** cmdlet.
The command passes the resource groups to the current cmdlet by using the pipeline operator.
The current cmdlet gets all deployments of all resource groups in the subscription, and passes the results to the Format-Table cmdlet to display their **ResourceGroupName**, **DeploymentName**, and **ProvisioningState** property values.

## PARAMETERS

### -ResourceGroupName
Specifies the name of a resource group.
The cmdlet gets the deployments for the resource group that this parameter specifies.
Wildcard characters are not permitted.
This parameter is required and you can specify only one resource group in each command.

```yaml
Type: String
Parameter Sets: The deployment name parameter set.
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the deployment to get.
Wildcard characters are not permitted.

```yaml
Type: String
Parameter Sets: The deployment name parameter set.
Aliases: DeploymentName

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApiVersion
Specifies the API version that is supported by the resource Provider.
You can specify a different version than the default version.

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

### -Id
Specifies the ID of the resource group deployment to get.

```yaml
Type: String
Parameter Sets: The deployment Id parameter set.
Aliases: DeploymentId, ResourceId

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Pre
Indicates that this cmdlet considers pre-release API versions when it automatically determines which version to use.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### Microsoft.Azure.Commands.ResourceManagement.Models.PSResourceGroupDeployment
The cmdlet returns resource group deployments.

## NOTES

## RELATED LINKS

[Get-AzureRmResourceGroup](./Get-AzureRmResourceGroup.md)

[New-AzureRmResourceGroup](./New-AzureRmResourceGroup.md)

[New-AzureRmResourceGroupDeployment](./New-AzureRmResourceGroupDeployment.md)

[Remove-AzureRmResourceGroupDeployment](./Remove-AzureRmResourceGroupDeployment.md)

[Stop-AzureRmResourceGroupDeployment](./Stop-AzureRmResourceGroupDeployment.md)

[Test-AzureRmResourceGroupDeployment](./Test-AzureRmResourceGroupDeployment.md)


