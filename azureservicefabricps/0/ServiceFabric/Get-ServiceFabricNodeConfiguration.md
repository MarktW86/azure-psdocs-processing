---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: B8FA0FAB-6ACB-4DA6-8A5B-AA871844DF77
online version:
schema: 2.0.0
updated_at: 05/01/2017 02:05 AM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/V5.6_Updates/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricNodeConfiguration.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/V5.6_Updates/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricNodeConfiguration.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/e91221cfb2152bc5747f2356d04a3cb4d6eeb59d
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
ms.service: service-fabric
---

# Get-ServiceFabricNodeConfiguration

## SYNOPSIS
Gets the configuration of a Service Fabric node.

## SYNTAX

```
Get-ServiceFabricNodeConfiguration [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricNodeConfiguration** cmdlet gets the configuration of a Service Fabric node.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

## EXAMPLES

### Example 1: Get node configuration
```
PS C:\> Get-ServiceFabricNodeConfiguration
```

This command returns the cluster manifest data corresponding to the node.

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

