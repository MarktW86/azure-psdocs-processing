---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/06/2017 14:04 PM
ms.date: 04/06/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/V5.6_Updates/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricRuntimeUpgradeVersion.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/V5.6_Updates/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricRuntimeUpgradeVersion.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/8cc7df560eb5276f5793b86a2b9d29aa7dfc34dd
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
ms.service: service-fabric
---

# Get-ServiceFabricRuntimeUpgradeVersion

## SYNOPSIS
Gets a list of all service fabric runtime versions which are upgrade compatible to a given version for standalone deployments.

## SYNTAX

```
Get-ServiceFabricRuntimeUpgradeVersion -BaseVersion <String> [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricRuntimeUpgradeVersion** cmdlet gets details about all upgradeable service fabric runtime versions for a given base version for standalone deployments.

The output of **Get-ServiceFabricRuntimeUpgradeVersion** contains the following information:

--Version: The service fabric runtime version.
--SupportExpiryDate : The date when the version goes out of support.      
--TargetPackageLocation : The link to download the runtime package.

## EXAMPLES

### Example 1
```
PS C:\> Get-ServiceFabricRuntimeUpgradeVersion -BaseVersion 5.4.164.9494
```

This command gets details about all service fabric runtime versions which can be upgraded to from version 5.4.164.9494.

## PARAMETERS

### -BaseVersion
Indicates the service fabric version for which all upgradeable versions need to be retreived.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeoutSec
Specifies the time-out period, in seconds, for the operation.

```yaml
Type: Int32
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
You cannot pipe input to this cmdlet.

## OUTPUTS

### System.Object
This cmdlet returns a List<Microsoft.ServiceFabric.DeploymentManager.Model.RuntimePackageDetails> which represents a list of all versions that can be upgraded to from a given BaseVersion.

## NOTES

## RELATED LINKS

[Get-ServiceFabricRuntimeSupportedVersion](./Get-ServiceFabricRuntimeSupportedVersion.md)

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[New-ServiceFabricCluster](./New-ServiceFabricCluster.md)

