---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: 13A0E0CC-38CE-4B64-8018-8DA8EFA7678B
online version:
schema: 2.0.0
updated_at: 05/19/2017 20:05 PM
ms.date: 05/19/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Restart-ServiceFabricDeployedCodePackage.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Restart-ServiceFabricDeployedCodePackage.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/8d4c81aabdfff50fd2bedea27942bd6899fa7bd1
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
---

# Restart-ServiceFabricDeployedCodePackage

## SYNOPSIS
Restarts a code package deployed on a node in a cluster to simulate a process failure.

## SYNTAX

### ByNodeName
```
Restart-ServiceFabricDeployedCodePackage [-NodeName] <String> [-ApplicationName] <Uri>
 [-ServiceManifestName] <String> [-CodePackageName] <String> [[-CodePackageInstanceId] <Int64>]
 [-ServicePackageActivationId <String>] [-CommandCompletionMode <CompletionMode>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### PartitionId
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -PartitionId <Guid> -ServiceName <Uri> [-TimeoutSec <Int32>] [<CommonParameters>]
```

### PartitionIdReplicaPrimary
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -PartitionId <Guid> -ServiceName <Uri> [-ReplicaKindPrimary] [-TimeoutSec <Int32>] [<CommonParameters>]
```

### PartitionIdReplicaRandomSecondary
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -PartitionId <Guid> -ServiceName <Uri> [-ReplicaKindRandomSecondary] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### PartitionIdReplicaId
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -PartitionId <Guid> -ServiceName <Uri> -ReplicaOrInstanceId <Int64> [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceName
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceNamePartitionSingleton
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindSingleton] [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceNamePartitionNamed
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindNamed] -PartitionKey <String> [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceNamePartitionUniformedInt
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindUniformInt64] -PartitionKey <String> [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### ServiceNamePartitionSingletonReplicaRandomSecondary
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindSingleton] [-ReplicaKindRandomSecondary] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### ServiceNamePartitionNamedReplicaRandomSecondary
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindNamed] -PartitionKey <String> [-ReplicaKindRandomSecondary]
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceNamePartitionUniformedIntReplicaRandomSecondary
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindUniformInt64] -PartitionKey <String> [-ReplicaKindRandomSecondary]
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceNamePartitionSingletonReplicaPrimary
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindSingleton] [-ReplicaKindPrimary] [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceNamePartitionNamedReplicaPrimary
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindNamed] -PartitionKey <String> [-ReplicaKindPrimary] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### ServiceNamePartitionUniformedIntReplicaPrimary
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindUniformInt64] -PartitionKey <String> [-ReplicaKindPrimary]
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceNamePartitionSingletonReplicaId
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindSingleton] -ReplicaOrInstanceId <Int64> [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### ServiceNamePartitionNamedReplicaId
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindNamed] -PartitionKey <String> -ReplicaOrInstanceId <Int64>
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceNamePartitionUniformedIntReplicaId
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-PartitionKindUniformInt64] -PartitionKey <String> -ReplicaOrInstanceId <Int64>
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceNameReplicaPrimary
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-ReplicaKindPrimary] [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceNameReplicaRandomSecondary
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> [-ReplicaKindRandomSecondary] [-TimeoutSec <Int32>] [<CommonParameters>]
```

### ServiceNameReplicaId
```
Restart-ServiceFabricDeployedCodePackage [-ApplicationName] <Uri> [-CommandCompletionMode <CompletionMode>]
 -ServiceName <Uri> -ReplicaOrInstanceId <Int64> [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Restart-ServiceFabricDeployedCodePackage** cmdlet ends the code package process, which restarts all of the user service replicas hosted in that process.
This restart simulates code package process failures in the cluster, which tests the failover recovery paths of your service.

You can specify a code package, or you can specify a ReplicaSelector to restart the node and code package combination where the replica is hosted.
This simplifies tests on the primary host node by not having to determine which Service Fabric node is the primary node before restarting that node.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

## EXAMPLES

### Example 1: Restart a code package for a random secondary replica
```
PS C:\> Restart-ServiceFabricDeployedCodePackage -ReplicaKindRandomSecondary -PartitionKindSingleton -ServiceName fabric:/SampleApp/SampleService -ApplicationName fabric:/SampleApp -CommandCompletionMode Verify
```

This command restarts a code package for a random secondary replica on a singleton partition.

### Example 2: Restart a specified code package
```
PS C:\> Restart-ServiceFabricDeployedCodePackage -NodeName "Node01" -ApplicationName fabric:/App -CodePackageName "CodePackage01" -ServiceManifestName "ServiceManifest01" -CommandCompletionMode Verify
```

This command restarts the code package named CodePackage01 from the service manifest named ServiceManifest01 on the node named Node01.

## PARAMETERS

### -ApplicationName
Specifies the name of the application to which the code package belongs.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -CodePackageInstanceId
Specifies the instance ID of the code package that is checked against the deployed one before restarting.
If you specify 0, no comparison is done.

```yaml
Type: Int64
Parameter Sets: ByNodeName
Aliases: 

Required: False
Position: 5
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -CodePackageName
Specifies the name of the code package to restart.

```yaml
Type: String
Parameter Sets: ByNodeName
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -CommandCompletionMode
Specifies whether the action waits for the restart to complete.

```yaml
Type: CompletionMode
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NodeName
Specifies the name of a Service Fabric node.
The cmdlet restarts the node you specify.

```yaml
Type: String
Parameter Sets: ByNodeName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PartitionId
Specifies the ID of the partition for which the code package is restarted.

```yaml
Type: Guid
Parameter Sets: PartitionId, PartitionIdReplicaPrimary, PartitionIdReplicaRandomSecondary, PartitionIdReplicaId
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PartitionKey
Specifies the key of the partition for which the code package is restarted.

```yaml
Type: String
Parameter Sets: ServiceNamePartitionNamed, ServiceNamePartitionUniformedInt, ServiceNamePartitionNamedReplicaRandomSecondary, ServiceNamePartitionUniformedIntReplicaRandomSecondary, ServiceNamePartitionNamedReplicaPrimary, ServiceNamePartitionUniformedIntReplicaPrimary, ServiceNamePartitionNamedReplicaId, ServiceNamePartitionUniformedIntReplicaId
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PartitionKindNamed
Indicates that this cmdlet restarts a code package on a named partition.

```yaml
Type: SwitchParameter
Parameter Sets: ServiceNamePartitionNamed, ServiceNamePartitionNamedReplicaRandomSecondary, ServiceNamePartitionNamedReplicaPrimary, ServiceNamePartitionNamedReplicaId
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartitionKindSingleton
Indicates that this cmdlet restarts a code package on a singleton partition.

```yaml
Type: SwitchParameter
Parameter Sets: ServiceNamePartitionSingleton, ServiceNamePartitionSingletonReplicaRandomSecondary, ServiceNamePartitionSingletonReplicaPrimary, ServiceNamePartitionSingletonReplicaId
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartitionKindUniformInt64
Indicates that this cmdlet restarts a code package on a UniformInt64 partition.

```yaml
Type: SwitchParameter
Parameter Sets: ServiceNamePartitionUniformedInt, ServiceNamePartitionUniformedIntReplicaRandomSecondary, ServiceNamePartitionUniformedIntReplicaPrimary, ServiceNamePartitionUniformedIntReplicaId
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReplicaKindPrimary
Indicates that this cmdlet restarts the code package for the primary replica.

```yaml
Type: SwitchParameter
Parameter Sets: PartitionIdReplicaPrimary, ServiceNamePartitionSingletonReplicaPrimary, ServiceNamePartitionNamedReplicaPrimary, ServiceNamePartitionUniformedIntReplicaPrimary, ServiceNameReplicaPrimary
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReplicaKindRandomSecondary
Indicates that this cmdlet restarts a code package for a random secondary replica.

```yaml
Type: SwitchParameter
Parameter Sets: PartitionIdReplicaRandomSecondary, ServiceNamePartitionSingletonReplicaRandomSecondary, ServiceNamePartitionNamedReplicaRandomSecondary, ServiceNamePartitionUniformedIntReplicaRandomSecondary, ServiceNameReplicaRandomSecondary
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReplicaOrInstanceId
Specifies a Service Fabric service replica or instance ID.

```yaml
Type: Int64
Parameter Sets: PartitionIdReplicaId, ServiceNamePartitionSingletonReplicaId, ServiceNamePartitionNamedReplicaId, ServiceNamePartitionUniformedIntReplicaId, ServiceNameReplicaId
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServiceManifestName
Specifies the name of the service manifest where the code package is defined.

```yaml
Type: String
Parameter Sets: ByNodeName
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServiceName
Specifies the name of the service to which the code package belongs.

```yaml
Type: Uri
Parameter Sets: PartitionId, PartitionIdReplicaPrimary, PartitionIdReplicaRandomSecondary, PartitionIdReplicaId, ServiceName, ServiceNamePartitionSingleton, ServiceNamePartitionNamed, ServiceNamePartitionUniformedInt, ServiceNamePartitionSingletonReplicaRandomSecondary, ServiceNamePartitionNamedReplicaRandomSecondary, ServiceNamePartitionUniformedIntReplicaRandomSecondary, ServiceNamePartitionSingletonReplicaPrimary, ServiceNamePartitionNamedReplicaPrimary, ServiceNamePartitionUniformedIntReplicaPrimary, ServiceNamePartitionSingletonReplicaId, ServiceNamePartitionNamedReplicaId, ServiceNamePartitionUniformedIntReplicaId, ServiceNameReplicaPrimary, ServiceNameReplicaRandomSecondary, ServiceNameReplicaId
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServicePackageActivationId
The activation id of the deployed *ServicePackage* which contain the *CodePackage*. This can be obtained by using the query [Get-ServiceFabricDeployedCodePackage](Get-ServiceFabricDeployedCodePackage.md).

If *ServicePackageActivationMode* specified at the time of creating the service (using [New-ServiceFabricService](New-ServiceFabricService.md)) is *SharedProcess* (or if it is not specfied, in which case it defaults to *SharedProcess*), then value of *ServicePackageActivationId* is always an empty string and need not be specified. To learn more about service package activation id, please see [Service Fabric Hosting Model][1].

```yaml
Type: String
Parameter Sets: ByNodeName
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
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

### System.Uri
Represents the name of a Service Fabric application.

### System.Uri
Represents the name of a Service Fabric service.

### System.Guid
Represents the ID of a Service Fabric partition.

## OUTPUTS

### string
Specifies the name of the Service Fabric service node.

## NOTES

## RELATED LINKS

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricDeployedCodePackage](./Get-ServiceFabricDeployedCodePackage.md)