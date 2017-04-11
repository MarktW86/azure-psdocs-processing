---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/11/2017 21:04 PM
ms.date: 04/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Add-AzureRMUsageConnection.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Add-AzureRMUsageConnection.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/da0fd350a2a76c2d3edbf597f3826de129c926e5
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
---

# Add-AzureRMUsageConnection

## SYNOPSIS
The Add-AzureRMUsageConnection cmdlet adds an usage connection details for a resource provider.
The cmdlet gets the storage account information where the resource provider is storing the usage records.
This information is given to the usage service through this cmdlet. 
Usage Service will retrieve the usage records periodically from the storage account information provided

## SYNTAX

```
Add-AzureRMUsageConnection -Name <String> -ResourceGroup <String> -ArmLocation <String>
 -ProviderLocation <String> -ProviderNamespace <String> -UsageStorageConnectionString <String>
 -UsageReportingQueue <String> -UsageReportingTable <String> -ErrorReportingQueue <String>
 -ErrorReportingTable <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-PipelineVariable <String>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Add-AzureRmUsageConnection @usageConnectionParams
```

Description

-----------

The following example registers a usage connection information of a resource provider to usage service

            $usageConnectionId = "sqlrpusageconnection"
            $location = "local"

            # Create Resource Group
            # The following name could be anything
            $usageConnectionRG="UsageConnectionRG"
            New-AzureRMResourceGroup -Name $usageConnectionRG  -Location $location -Force

            # Make sure the tables and queues exist
            # if not create them with New-AzureStorageTale/New-AzureStorageQueue
            $usageReportingQueue = "sqlrpusagequeue"
            $usageReportingTable = "sqlrpusagetable"
            $errorReportingQueue = "sqlrpusageerrorqueue"
            $errorReportingTable = "sqlrpusageerrortable"

            # Create Storage Account If Other than DevStorage
            $storageConnectionString = "UseDevelopmentStorage=true"


            $usageConnectionParams = @{
            Name = $usageConnectionId
            ResourceGroup = $usageConnectionRG
            ProviderNamespace = "Microsoft.Sql"
            ArmLocation = $location
            ProviderLocation = $location
            UsageStorageConnectionString = $storageConnectionString
            UsageReportingQueue = $usageReportingQueue
            UsageReportingTable = $usageReportingTable
            ErrorReportingQueue = $errorReportingQueue
            ErrorReportingTable = $errorReportingTable
            ApiVersion = "2015-06-01-preview"
            }

            Add-AzureRmUsageConnection @usageConnectionParams

## PARAMETERS

### -ArmLocation
This is the Location of the resource manager instance in the Azure Stack installation

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

### -ErrorReportingQueue
Queue name for reporting the errors.
Usage service would insert records in this queue for any errors during its collection process

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorReportingTable
Table name for reporting the errors.
Usage service would insert records in this queue for any errors during its collection process

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
Not Specified

The following values are permitted for this object type.

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa
Accepted values: SilentlyContinue, Stop, Continue, Inquire

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Not Specified

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the usage connection

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PipelineVariable
Not Specified

```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProviderLocation
Location of the resource provider for which the usage connection is being added

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ProviderNamespace
Namespace of the resource provider for which the usage connection is being added

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroup
Resource group name for the usage connection resource

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UsageReportingQueue
Queue name where the added usage meta data is queued .
Using this metadata, Usage service will read the data from reporting table for usage aggregation

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UsageReportingTable
Table name where usage records are inserted

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UsageStorageConnectionString
This specifies the storage connection string in which the resource provider usage records are inserted

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.AzureStack.Management.Models.UsageConnectionModel

## NOTES

## RELATED LINKS

