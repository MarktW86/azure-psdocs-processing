---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: 50612BDC-6E73-47E4-A4DB-DE8CF804BB85
updated_at: 11/01/2016 22:11 PM
ms.date: 11/01/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/DuncanmaMSFT-patch-1/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v2.1.0/Get-AzureRmWebApp.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/DuncanmaMSFT-patch-1/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v2.1.0/Get-AzureRmWebApp.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: Websites
---

# Get-AzureRmWebApp

## SYNOPSIS
Gets Azure Web Apps in the specified resource group.

## SYNTAX

### S1
```
Get-AzureRmWebApp [[-ResourceGroupName] <String>] [[-Name] <String>] [<CommonParameters>]
```

### S2
```
Get-AzureRmWebApp [-AppServicePlan] <ServerFarmWithRichSku> [<CommonParameters>]
```

### S3
```
Get-AzureRmWebApp [-Location] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmWebApp** cmdlet gets information about Azure Web Apps in the specified resource group.

## EXAMPLES

### Example 1: Get a Web App from a resource group
```
PS C:\>Get-AzureRmWebApp -ResourceGroupName "Default-Web-WestUS" -Name "WebAppStandard" -SlotName "Slot001"
```

This command gets the slot named Slot001 from the Web App named WebAppStandard that belongs to the resource group Default-Web-WestUS.

## PARAMETERS

### -ResourceGroupName

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name

```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -AppServicePlan

```yaml
Type: ServerFarmWithRichSku
Parameter Sets: S2
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Location

```yaml
Type: String
Parameter Sets: S3
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureRmWebApp](./New-AzureRmWebApp.md)

[Remove-AzureRmWebApp](./Remove-AzureRmWebApp.md)

[Restart-AzureRmWebApp](./Restart-AzureRmWebApp.md)

[Start-AzureRmWebApp](./Start-AzureRmWebApp.md)

[Stop-AzureRmWebApp](./Stop-AzureRmWebApp.md)


