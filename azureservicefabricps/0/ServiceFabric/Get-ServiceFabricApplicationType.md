---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: 377D093A-8D81-4CDA-842B-EF8A9FF2585C
online version:
schema: 2.0.0
updated_at: 05/22/2017 16:05 PM
ms.date: 05/22/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricApplicationType.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricApplicationType.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/4e8238593aaaa3791768101915784440753ab117
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
ms.service: service-fabric
---

# Get-ServiceFabricApplicationType

## SYNOPSIS
Gets the Service Fabric application types registered on the Service Fabric cluster which match the provided filters.

## SYNTAX

```
Get-ServiceFabricApplicationType [[-ApplicationTypeName] <String>] [-ExcludeApplicationParameters] [-UsePaging]
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricApplicationType** cmdlet gets the Service Fabric application types registered or registering on the Service Fabric cluster which match the provided filters. Each version of an application type is returned as an individual result in the result array. If no application types are found matching the provided parameters, this query does not return anything.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

## EXAMPLES

### Example 1: Get all registered or registering application types
```
PS C:\> Get-ServiceFabricApplicationType
```

This command gets all registered application types.	

### Example 2: Get registered or registering application type with specified type names
```
PS C:\> # Scenario: multiple application types are provisioned in the cluster, including TestApp versions 1 and 2, as well as TestApp2 version 1.
PS C:\> Get-ServiceFabricApplicationType -ApplicationTypeName "TestApp"
```

This command gets all the versions of the application type "TestApp". This does not get the application type "TestApp2" because the application type name is not an exact match.

### Example 3: Get all registered or registering application types without default application parameters
```
PS C:\>Get-ServiceFabricApplicationType -ExcludeApplicationParameters
```

This command gets all registered application types. The returned [System.Fabric.Query.ApplicationType](/dotnet/api/system.fabric.query.applicationtype) object(s) have an unpopulated DefaultParameters property, regardless of whether the application type has default application parameters.

### Example 4: Get all registered or registering application types with paging and then piping
```
PS C:\> Get-ServiceFabricApplicationType -UsePaging | Get-ServiceFabricApplicationManifest
```

This command gets all registered or registering application types using paging. This means that messages are not dropped if they do not fit into one message, whose size is determined by the max messaage size configuration. Paging is done behind the scenes by the query. Piping and other functionality remains unchanged.

## PARAMETERS

### -ApplicationTypeName
Specifies the name of a Service Fabric application type. The cmdlet gets all versions of the application type that you specify.

If you do not specify this parameter, this cmdlet gets all application types. This parameter matches against the case sensitive exact application type names defined in the application manifest of all provisioned or provisioning application types. For example, the value "Test" does not match "TestApp" because it is only a partial match. This value should not contain the version of the application type, and matches all versions of the same application type name.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ExcludeApplicationParameters
Specifies whether to exclude default application parameters from the query result. 

If set, the default application parameters field is still visible, but is empty.

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

### -UsePaging
Specifies whether to use a paged version of this query.

If this query is unpaged, the number of returned results is restricted by the max message size configuration. If not specified and there are too many application types to fit into a message, the query fails. No results are returned to the user. If the query is paged, then results are not dropped due to message size contraints because the results are broken up into pages when needed and looped through. Paging is done internally by the query, and no additional steps are required.

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

### String
This cmdlet accepts a string that represents the application type name filter.

## OUTPUTS

### System.Array
An Object[] with each object being a [System.Fabric.Query.ApplicationType](/dotnet/api/system.fabric.query.applicationtype) object that represents the Service Fabric application types in case of multiple returned application types.

### System.Object
A [System.Fabric.Query.ApplicationType](/dotnet/api/system.fabric.query.applicationtype) object in case of a single returned application type.

## NOTES

## RELATED LINKS

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)

[Register-ServiceFabricApplicationType](./Register-ServiceFabricApplicationType.md)

[Unregister-ServiceFabricApplicationType](./Unregister-ServiceFabricApplicationType.md)
