---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/24/2017 22:05 PM
ms.date: 05/24/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.1.3/Start-AzureRmWebApp.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.1.3/Start-AzureRmWebApp.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/2d4a4fe807f8dce278c44747fc746934ed66d9fe
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: Websites
---

# Start-AzureRmWebApp

## SYNOPSIS
Starts a web app.

## SYNTAX

### S1
```
Start-AzureRmWebApp [-ResourceGroupName] <String> [-Name] <String> [<CommonParameters>]
```

### S2
```
Start-AzureRmWebApp [-WebApp] <Site> [<CommonParameters>]
```

## DESCRIPTION
The **Start-AzureRmWebApp** cmdlet starts a web app that was built using the Web Apps feature of the Azure App Service.

## EXAMPLES

### Example 1: Start a web app
```
Start-AzureRmWebApp -ResourceGroupName "Default-Web-WestUS" -Name "ContosoWebApp"
```

This example starts the web app named "ContosoWebApp" that belongs to the resource group named "Default-Web-WestUS".

## PARAMETERS

### -Name
Specifies the name of the web app to start.

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
Specifies the name of the resource group that contains the web app to start.

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

### -WebApp
Specifies a **WebApp** object that contains details about the web app to start.

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

[Get-AzureRmWebApp](./Get-AzureRmWebApp.md)

[New-AzureRmWebApp](./New-AzureRmWebApp.md)

[Remove-AzureRmWebApp](./Remove-AzureRmWebApp.md)

[Restart-AzureRmWebApp](./Restart-AzureRmWebApp.md)

[Stop-AzureRmWebApp](./Stop-AzureRmWebApp.md)
