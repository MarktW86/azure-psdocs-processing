---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: 180D2ECE-79F6-4047-99D6-5D987A90AE88
online version:
schema: 2.0.0
updated_at: 05/01/2017 01:05 AM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/V5.6_Updates/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricServiceGroupMember.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/V5.6_Updates/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricServiceGroupMember.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/05f3c2c9a589d42a19142269eb3dc35b4e30270a
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
ms.service: service-fabric
---

# Get-ServiceFabricServiceGroupMember

## SYNOPSIS
Gets members of service groups.

## SYNTAX

### Non-Adhoc (Default)
```
Get-ServiceFabricServiceGroupMember [-ApplicationName] <Uri> [[-ServiceName] <Uri>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### Adhoc
```
Get-ServiceFabricServiceGroupMember [-Adhoc] [[-ServiceName] <Uri>] [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricServiceGroupMember** cmdlet gets members of Service Fabric service groups.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

## EXAMPLES

### Example 1: Get a service group members
```
PS C:\> Get-ServiceFabricServiceGroupMember -ApplicationName -ServiceName fabric:/CalcApp
```

The command gets Service Fabric service group members for the service named fabric:/CalcApp.

## PARAMETERS

### -Adhoc
Indicates that the service runs in ad hoc mode.
In ad hoc mode, you manually activate the service host.

```yaml
Type: SwitchParameter
Parameter Sets: Adhoc
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApplicationName
Specifies the Uniform Resource Identifier (URI) of a Service Fabric application.
This cmdlet gets group members for the application that this parameter specifies.

```yaml
Type: Uri
Parameter Sets: Non-Adhoc
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServiceName
Specifies the Uniform Resource Identifier (URI) of a Service Fabric service group.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Uri
This cmdlet accepts a URI that represents the name of a Service Fabric application or the name of a Service Fabric service group.

## OUTPUTS

### System.Object
This cmdlet returns a list of **System.Fabric.Query.ServiceGroupMember** objects that represent Service Fabric service group members.

## NOTES

## RELATED LINKS

[Get-ServiceFabricServiceGroupMemberType](./Get-ServiceFabricServiceGroupMemberType.md)

[New-ServiceFabricServiceGroup](./New-ServiceFabricServiceGroup.md)

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)
