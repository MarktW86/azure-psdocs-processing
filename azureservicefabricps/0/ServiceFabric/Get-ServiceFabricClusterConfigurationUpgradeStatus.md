---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: F39A8721-65AC-449E-A0F6-4C9AA22E9029
online version:
schema: 2.0.0
updated_at: 05/03/2017 21:05 PM
ms.date: 05/03/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/Graham71141/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricClusterConfigurationUpgradeStatus.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/Graham71141/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricClusterConfigurationUpgradeStatus.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/50b4a1d8c941cfe43b0ae98efc047bbdc78270fd
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
ms.service: service-fabric
---

# Get-ServiceFabricClusterConfigurationUpgradeStatus

## SYNOPSIS
Gets the status for Service Fabric cluster configuration upgrade.

## SYNTAX

```
Get-ServiceFabricClusterConfigurationUpgradeStatus [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricClusterConfigurationUpgradeStatus** cmdlet gets the current configuration upgrade status.

## EXAMPLES

### Example 1: Get update status
```
PS C:\> Get-ServiceFabricClusterConfiguratoinUpgradeStatus
```

This cmdlet gets current configuration update status.

## PARAMETERS

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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-ServiceFabricClusterConfiguration](./Get-ServiceFabricClusterConfiguration.md)

[Start-ServiceFabricClusterConfigurationUpgrade](./Start-ServiceFabricClusterConfigurationUpgrade.md)


