---
external help file: Microsoft.Azure.Commands.IotHub.dll-Help.xml
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/IotHub/Commands.IotHub/help/Get-AzureRmIotHubEventHubConsumerGroup.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/IotHub/Commands.IotHub/help/Get-AzureRmIotHubEventHubConsumerGroup.md
gitcommit: https://github.com/Azure/azure-powershell/blob/04e47f8329ba9e64790c974f9666dbf41de7483f
updated_at: 06/08/2017 20:06 PM
ms.date: 06/08/2017
ms.topic: reference
---

# Get-AzureRmIotHubEventHubConsumerGroup

## SYNOPSIS
Gets all the eventhub consumergroups.

## SYNTAX

```
Get-AzureRmIotHubEventHubConsumerGroup [-ResourceGroupName] <String> [-Name] <String>
 [-EventHubEndpointName] <String> [<CommonParameters>]
```

## DESCRIPTION
Gets all the eventhub consumergroups for the different EventHubs used by IotHub.

## EXAMPLES

### Example 1 Gets all the eventhub consumergroups for the telemetry eventhub
```
PS C:\> Get-AzureRmIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubEndpointName "events"
```

Gets all the eventhub consumergroups for the telemetry eventhub for the iothub named myiothub

### Example 2 Gets all the eventhub consumergroups for the operationsmonitoring eventhub
```
PS C:\> Get-AzureRmIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubEndpointName "operationsMonitoringEvents"
```

Gets all the eventhub consumergroups for the operationsMonitoringEvents eventhub for the iothub named myiothub

## PARAMETERS

### -EventHubEndpointName
Name of the Event Hub endpoint.
Possible values events, operationsMonitoringEvents

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

### -Name
Name of the IotHub

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

### -ResourceGroupName
Resource Group Name

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### System.Collections.Generic.IEnumerable`1[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]

## NOTES

## RELATED LINKS

