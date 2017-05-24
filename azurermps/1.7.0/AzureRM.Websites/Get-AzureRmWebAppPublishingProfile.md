---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/24/2017 22:05 PM
ms.date: 05/24/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.1.3/Get-AzureRmWebAppPublishingProfile.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.1.3/Get-AzureRmWebAppPublishingProfile.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/2d4a4fe807f8dce278c44747fc746934ed66d9fe
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: Websites
---

# Get-AzureRmWebAppPublishingProfile

## SYNOPSIS
Gets the publishing profile of a web app.

## SYNTAX

### S1
```
Get-AzureRmWebAppPublishingProfile [-OutputFile] <String> [[-Format] <String>] [-ResourceGroupName] <String>
 [-Name] <String> [<CommonParameters>]
```

### S2
```
Get-AzureRmWebAppPublishingProfile [-OutputFile] <String> [[-Format] <String>] [-WebApp] <Site>
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmWebAppPublishingProfile** cmdlet gets the publishing profile of a web app that was built using the Web Apps feature of the Azure App Service.

## EXAMPLES

### Example 1: Get the publishing profile in "Ftp" format
```
Get-AzureRmWebAppSlotPublishingProfile -ResourceGroupName "Default-Web-WestUS" -Name "ContosoWebApp" -Format "Ftp" -OutputFile "C:\Users\contoso\outputfile"
```

This example gets the publishing profile in "Ftp" format for a web app named "ContosoWebApp" in the "Default-Web-WestUS" resource group.
The profile is stored in "C:\Users\contoso\outputfile".

## PARAMETERS

### -Format
Specifies the output format for the publishing profile.
Valid values are "FileZilla3", "WebDeploy", and "Ftp".

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the web app for which to get the publishing profile.

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

### -OutputFile
Specifies the name of the file in which to output the publishing profile.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
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

[Get-AzureRmAppServicePlan](./Get-AzureRmAppServicePlan.md)

[Get-AzureRmWebApp](./Get-AzureRmWebApp.md)
