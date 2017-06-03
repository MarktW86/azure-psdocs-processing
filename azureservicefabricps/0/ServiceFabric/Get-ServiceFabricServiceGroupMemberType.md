---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: F0140597-B5F1-4DA7-B5FC-CFA447FA6F5A
online version:
schema: 2.0.0
updated_at: 05/19/2017 20:05 PM
ms.date: 05/19/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricServiceGroupMemberType.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricServiceGroupMemberType.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/8d4c81aabdfff50fd2bedea27942bd6899fa7bd1
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
ms.service: service-fabric
---

# Get-ServiceFabricServiceGroupMemberType

## SYNOPSIS
Gets member types of Service Fabric service groups.

## SYNTAX

```
Get-ServiceFabricServiceGroupMemberType [-ApplicationTypeName] <String> [-ApplicationTypeVersion] <String>
 [[-ServiceGroupTypeName] <String>] [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricServiceGroupMemberType** cmdlet gets member types of Service Fabric service groups.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

## EXAMPLES

### Example 1: Get a service group member types
```
PS C:\> Get-ServiceFabricServiceGroupMemberType -ApplicationTypeName "CalcApp" -ApplicationTypeVersion "1.0"
```

This command gets Service Fabric service group member types for the application type named CalcApp and application type version 1.0.

## PARAMETERS

### -ApplicationTypeName
Specifies the name of a Service Fabric application type.
The cmdlet gets types for the application type that this parameter specifies.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApplicationTypeVersion
Specifies the version of a Service Fabric application type.
The cmdlet gets types for the application version that this parameter specifies.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServiceGroupTypeName
Specifies the name of a service group type.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
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

### String
This cmdlet accepts the name of a Service Fabric application type, an application type version, or the name of a service group.

## OUTPUTS

### System.Object
This cmdlet returns a list of **System.Fabric.Query.ServiceGroupMemberType** objects that represent Service Fabric service group member types.

## NOTES

## RELATED LINKS

[Get-ServiceFabricServiceGroupMember](./Get-ServiceFabricServiceGroupMember.md)

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)
