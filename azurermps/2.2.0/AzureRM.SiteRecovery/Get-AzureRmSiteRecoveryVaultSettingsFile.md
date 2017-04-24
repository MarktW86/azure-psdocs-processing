---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: C2A2C222-136A-42B1-9312-14F29CA68586
updated_at: 11/11/2016 23:11 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71305/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v2.1.0/Get-AzureRmSiteRecoveryVaultSettingsFile.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71305/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v2.1.0/Get-AzureRmSiteRecoveryVaultSettingsFile.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: site-recovery
---

# Get-AzureRmSiteRecoveryVaultSettingsFile

## SYNOPSIS
Gets the Site Recovery vault settings file.

## SYNTAX

### ByParam (Default)
```
Get-AzureRmSiteRecoveryVaultSettingsFile [<CommonParameters>]
```

### Default
```
Get-AzureRmSiteRecoveryVaultSettingsFile -Vault <ASRVault> [-Path <String>] [<CommonParameters>]
```

### ForSite
```
Get-AzureRmSiteRecoveryVaultSettingsFile -Vault <ASRVault> -SiteIdentifier <String> -SiteFriendlyName <String>
 [-Path <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmSiteRecoveryVaultSettingsFile** cmdlet gets the settings file for an Azure Site Recovery vault.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Path
Specifies the path to the Site Recovery vault settings file.
To store this file locally, download it from the Site Recovery vault portal once the command completes.

```yaml
Type: String
Parameter Sets: Default, ForSite
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteFriendlyName
Specifies the site friendly name for the vault when the site is a Hyper-V site.

```yaml
Type: String
Parameter Sets: ForSite
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteIdentifier
Specifies the site identifier for the vault when the site is a Hyper-V site.

```yaml
Type: String
Parameter Sets: ForSite
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Vault
Specifies the vault object for the site.

```yaml
Type: ASRVault
Parameter Sets: Default, ForSite
Aliases: 

Required: True
Position: Named
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

[Import-AzureRmSiteRecoveryVaultSettingsFile](./Import-AzureRmSiteRecoveryVaultSettingsFile.md)

[Set-AzureRmSiteRecoveryVaultSettings](./Set-AzureRmSiteRecoveryVaultSettings.md)


