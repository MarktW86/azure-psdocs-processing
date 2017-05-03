---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: 4275CC75-BDDD-4782-99C8-D3E775F07E61
online version:
schema: 2.0.0
updated_at: 05/03/2017 06:05 AM
ms.date: 05/03/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/V5.6_Updates/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricService.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/V5.6_Updates/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricService.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/40385fc07259a8f5f0d2cec04a231e9cd42fcff3
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
ms.service: service-fabric
---

# Get-ServiceFabricService

## SYNOPSIS
Gets a list of Service Fabric services.

## SYNTAX

### Non-Adhoc (Default)
```
Get-ServiceFabricService [-ApplicationName] <Uri> [[-ServiceName] <Uri>] [-ServiceTypeName <String>]
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

### Adhoc
```
Get-ServiceFabricService [-Adhoc] [[-ServiceName] <Uri>] [-ServiceTypeName <String>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricService** cmdlet gets a list of Service Fabric services.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

## EXAMPLES

### Example 1: Get the services created from an application
```
PS C:\> Get-ServiceFabricService -ApplicationName fabric:/myapp/persistenttodolist
```

This command gets the Service Fabric services from the specified application.

### Example 2: Get the system services running in a cluster
```
PS C:\> Get-ServiceFabricService -ApplicationName fabric:/System
```

This command gets the Service Fabric system services running in a cluster.

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
The cmdlet gets the services for the applications that you specify.

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
Specifies the URI of a Service Fabric service.
If you do not specify this parameter, this cmdlet gets all services of the specified application.

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

### -ServiceTypeName
{{Fill ServiceTypeName Description}}

```yaml
Type: String
Parameter Sets: (All)
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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Uri
This cmdlet accept a URI that represents the name of a Service Fabric application or the name of a Service Fabric service.

## OUTPUTS

### System.Object
This cmdlet returns a list of **[System.Fabric.Query.Service](https://docs.microsoft.com/en-us/dotnet/api/system.fabric.query.service)** objects that represent Service Fabric services.

## NOTES

## RELATED LINKS

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)

[New-ServiceFabricService](./New-ServiceFabricService.md)

[Remove-ServiceFabricService](./Remove-ServiceFabricService.md)

[Resolve-ServiceFabricService](./Resolve-ServiceFabricService.md)

[Update-ServiceFabricService](./Update-ServiceFabricService.md)
