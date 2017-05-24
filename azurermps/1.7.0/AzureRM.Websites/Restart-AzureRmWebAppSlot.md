---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/24/2017 22:05 PM
ms.date: 05/24/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.1.3/Restart-AzureRmWebAppSlot.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.1.3/Restart-AzureRmWebAppSlot.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/2d4a4fe807f8dce278c44747fc746934ed66d9fe
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: Websites
---

# Restart-AzureRmWebAppSlot

## SYNOPSIS
Stops and then restarts a web app slot.

## SYNTAX

### S1
```
Restart-AzureRmWebAppSlot [-ResourceGroupName] <String> [-Name] <String> [-Slot] <String> [<CommonParameters>]
```

### S2
```
Restart-AzureRmWebAppSlot [-WebApp] <Site> [<CommonParameters>]
```

## DESCRIPTION
The **Restart-AzureRmWebAppSlot** cmdlet stops and then restarts a web app slot.
If the web app slot is in a stopped state, use the **Start-AzureRmWebAppSlot** cmdlet to start the web app slot.


## EXAMPLES

### Example 1: Restart a web app slot
```
Restart-AzureRmWebAppSlot -ResourceGroupName "Default-Web-WestUS" -Name "ContosoWebApp" -Slot "Slot001"
```

This example restarts the slot named "Slot001" for the web app named "ContosoWebApp" that is in the "Default-Web-WestUS" resource group.

## PARAMETERS

### -Name
Specifies the name of the web app.

```yaml
Type: String
Parameter Sets: S1
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that contains the web app.

```yaml
Type: String
Parameter Sets: S1
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Slot
Specifies the name of the slot to restart.

```yaml
Type: String
Parameter Sets: S1
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebApp
Specifies a **WebApp** object that contains details about the web app.

```yaml
Type: Site
Parameter Sets: S2
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRMWebAppSlot](./Get-AzureRMWebAppSlot.md)

[New-AzureRMWebAppSlot](./New-AzureRMWebAppSlot.md)

[Remove-AzureRMWebAppSlot](./Remove-AzureRMWebAppSlot.md)

[Set-AzureRMWebAppSlot](./Set-AzureRMWebAppSlot.md)

[Start-AzureRMWebAppSlot](./Start-AzureRMWebAppSlot.md)

[Stop-AzureRMWebAppSlot](./Stop-AzureRMWebAppSlot.md)

[Get-AzureRmWebApp](./Get-AzureRmWebApp.md)
