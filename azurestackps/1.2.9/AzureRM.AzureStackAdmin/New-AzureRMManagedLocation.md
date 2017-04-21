---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/11/2017 21:04 PM
ms.date: 04/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/staging/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/New-AzureRMManagedLocation.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/staging/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/New-AzureRMManagedLocation.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/da0fd350a2a76c2d3edbf597f3826de129c926e5
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# New-AzureRMManagedLocation

## SYNOPSIS
The cmdlet New-AzureRmManagedLocation creates a new location managed by Azurestack Resource Manager.
The resource providers can be deployed in the new location

## SYNTAX

```
New-AzureRMManagedLocation -Name <String> -DisplayName <String> -Latitude <Double> -Longitude <Double>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-PipelineVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
New-AzureRMManagedLocation -Name "LocationName" -DisplayName "LocationName" -Latitude 80.5 -Longitude -45.5
```

Description

-----------

The example creates a new location

## PARAMETERS

### -DisplayName
@{Text=}

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

### -Latitude
Specifies the latitude of the location in decimal format

```yaml
Type: Double
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Longitude
Specifies the Longitude of the location in decimal format

```yaml
Type: Double
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the location

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.AzureStack.Management.Models.Location

## NOTES

## RELATED LINKS

