---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/24/2017 22:05 PM
ms.date: 05/24/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.1.3/Remove-AzureRmWebAppSlot.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.1.3/Remove-AzureRmWebAppSlot.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/2d4a4fe807f8dce278c44747fc746934ed66d9fe
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: Websites
---

# Remove-AzureRmWebAppSlot

## SYNOPSIS
Removes a web app slot.

## SYNTAX

### S1
```
Remove-AzureRmWebAppSlot [-Force] [-ResourceGroupName] <String> [-Name] <String> [-Slot] <String> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### S2
```
Remove-AzureRmWebAppSlot [-Force] [-WebApp] <Site> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmWebAppSlot** cmdlet removes a slot for a web app that was built using the Web Apps feature of the Azure App Service.

## EXAMPLES

### Example 1: Remove a web app slot
```
Remove-AzureRmWebAppSlot -ResourceGroupName "Default-Web-WestUS" -Name "ContosoSite" -Slot "Slot001"
```

This example removes the slot named "Slot001" associated with the web app "ContosoSite" that is in the "Default-Web-WestUS" resource group.

## PARAMETERS

### -Force
Indicates whether to forcefully remove the slot.

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
Specifies the name of the slot to remove.

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

### -Confirm
Indicates whether to prompt the user for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Indicates whether to show what would happen if the cmdlet runs without actually running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

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

## NOTES

## RELATED LINKS

[Get-AzureRMWebAppSlot](./Get-AzureRMWebAppSlot.md)

[New-AzureRMWebAppSlot](./New-AzureRMWebAppSlot.md)

[Restart-AzureRMWebAppSlot](./Restart-AzureRMWebAppSlot.md)

[Set-AzureRMWebAppSlot](./Set-AzureRMWebAppSlot.md)

[Start-AzureRMWebAppSlot](./Start-AzureRMWebAppSlot.md)

[Stop-AzureRMWebAppSlot](./Stop-AzureRMWebAppSlot.md)

[Get-AzureRmWebApp](./Get-AzureRmWebApp.md)
