---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: 9D683253-3A20-4F8D-98CC-8C1CFE455546
online version:
schema: 2.0.0
updated_at: 05/19/2017 20:05 PM
ms.date: 05/19/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Remove-ServiceFabricTestState.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Remove-ServiceFabricTestState.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/8d4c81aabdfff50fd2bedea27942bd6899fa7bd1
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
---

# Remove-ServiceFabricTestState

## SYNOPSIS
Removes all test state data from a Service Fabric cluster.

## SYNTAX

```
Remove-ServiceFabricTestState [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-ServiceFabricTestState** cmdlet removes all of the test state data from a Service Fabric cluster.
You can use this cmdlet in the case of a bad shutdown of the test driver.
Some actions set test state in the Service Fabric cluster, and if the process fails while in this state, it could leave the Service Fabric cluster unusable.
The **Remove-ServiceFabricTestState** clears this test state data.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

## EXAMPLES

### Example 1: Remove a Service Fabric test state
```
PS C:\> Remove-ServiceFabricTestState
```

This command removes the Service Fabric test state.

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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

###  
None.

## OUTPUTS

### System.Object
This cmdlet returns a **String** object that represents the final status of the clean operation.

## NOTES

## RELATED LINKS

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Test-ServiceFabricApplication](./Test-ServiceFabricApplication.md)
