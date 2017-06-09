---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 06/08/2017 17:06 PM
ms.date: 06/08/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricRuntimeSupportedVersion.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricRuntimeSupportedVersion.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/22ccbdbe6f5398c7882b9dcbcefafd417548cbdb
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
---

# Get-ServiceFabricRuntimeSupportedVersion

## SYNOPSIS
Gets a list of all currently supported service fabric runtime versions for standalone deployments.

## SYNTAX

```
Get-ServiceFabricRuntimeSupportedVersion [-Latest] [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricRuntimeSupportedVersion** cmdlet gets details about all currently supported service fabric runtime versions for standalone deployments.

The output of **Get-ServiceFabricRuntimeSupportedVersion** contains the following information:

-Version: The service fabric runtime version.
-SupportExpiryDate : The date when the version goes out of support.      
-TargetPackageLocation : The link to download the runtime package.

## EXAMPLES

### Example 1
```
PS C:\> Get-ServiceFabricRuntimeSupportedVersion
```

This command gets details about all supported service fabric runtime versions for standalone deployments.

### Example 2
```
PS C:\> Get-ServiceFabricRuntimeSupportedVersion -Latest
```

This command gets details about the latest supported service fabric runtime version for standalone deployments.

## PARAMETERS

### -Latest
Indicates that the command returns only the latest version details.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
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
This cmdlet returns a List<Microsoft.ServiceFabric.DeploymentManager.Model.RuntimePackageDetails> that represents a list of all supported runtime version details.

## NOTES

## RELATED LINKS

[Get-ServiceFabricRuntimeUpgradeVersion](./Get-ServiceFabricRuntimeUpgradeVersion.md)

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[New-ServiceFabricCluster](./New-ServiceFabricCluster.md)
