---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
ms.assetid: BBC85035-DCF7-44FA-A747-A1563A55B820
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Websites/Commands.Websites/help/Get-AzureRmWebAppBackupList.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Websites/Commands.Websites/help/Get-AzureRmWebAppBackupList.md
gitcommit: https://github.com/Azure/azure-powershell/blob/188033f88f70f578d4879e2a78bf41bbfbaeaf0c
updated_at: 04/28/2017 07:04 AM
ms.date: 04/28/2017
ms.topic: reference
---

# Get-AzureRmWebAppBackupList

## SYNOPSIS

## SYNTAX

### FromResourceName
```
Get-AzureRmWebAppBackupList [-ResourceGroupName] <String> [-Name] <String> [[-Slot] <String>]
 [<CommonParameters>]
```

### FromWebApp
```
Get-AzureRmWebAppBackupList [-WebApp] <Site> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmWebAppBackupList** cmdlet gets a list of backups for an Azure Web App.

## EXAMPLES

### 1:
```
PS C:\>Get-AzureRmWebAppBackupList -ResourceGroupName "Default-Web-WestUS" -Name "WebAppStandard"
```

This command returns a backup list pertaining to WebApp WebAppStandard associated with the resource group ContosoResourceGroup.

## PARAMETERS

### -ResourceGroupName
Resource Group Name

```yaml
Type: String
Parameter Sets: FromResourceName
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
WebApp Name

```yaml
Type: String
Parameter Sets: FromResourceName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
Slot name

```yaml
Type: String
Parameter Sets: FromResourceName
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -WebApp
Piped WebApp

```yaml
Type: Site
Parameter Sets: FromWebApp
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

