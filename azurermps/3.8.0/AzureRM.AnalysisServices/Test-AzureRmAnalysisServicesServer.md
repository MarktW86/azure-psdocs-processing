---
external help file: Microsoft.Azure.Commands.AnalysisServices.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/07/2017 09:04 AM
ms.date: 04/07/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.AnalysisServices/v0.2.0/Test-AzureRmAnalysisServicesServer.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.AnalysisServices/v0.2.0/Test-AzureRmAnalysisServicesServer.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/195dcb690a30a5f2c0ecd5606483862547ef544a
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
---

# Test-AzureRmAnalysisServicesServer

## SYNOPSIS
Tests the existence of an instance of Analysis Services server

## SYNTAX

```
Test-AzureRmAnalysisServicesServer [-Name] <String> [[-ResourceGroupName] <String>]
```

## DESCRIPTION
The Test-AzureRmAnalysisServicesServer cmdlet tests the existence of an instance of Analysis Services server

## EXAMPLES

### Example 1
```
PS C:\> Test-AzureRmAnalysisServicesServer -Name "testserver" -ResourceGroupName "testgroup"
```

This command will test if there is a server named testserver in the resourcegroup testgroup

## PARAMETERS

### -Name
Name of the Analysis Services server

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

### -ResourceGroupName
Name of the Azure resource group to which the server belongs

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

## INPUTS

## OUTPUTS

### System.Boolean

## NOTES
Alias: Test-AzureAs

## RELATED LINKS

[Get-AzureRmAnalysisServicesServer](./Get-AzureRmAnalysisServicesServer.md)

[Remove-AzureRmAnalysisServicesServer](./Remove-AzureRmAnalysisServicesServer.md)