---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
ms.assetid: C4C624DB-BBE8-4F94-BDC6-C012482F7271
online version:
schema: 2.0.0
updated_at: 05/11/2017 18:05 PM
ms.date: 05/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v4.0.0/Remove-AzureRmSiteRecoveryPolicy.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v4.0.0/Remove-AzureRmSiteRecoveryPolicy.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a9b160b3b332c6a38589f1828b17cf2391c2454e
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: site-recovery
---

# Remove-AzureRmSiteRecoveryPolicy

## SYNOPSIS
Removes a Site Recovery replication policy.

## SYNTAX

```
Remove-AzureRmSiteRecoveryPolicy -Policy <ASRPolicy> [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRMSiteRecoveryPolicy** cmdlet removes an Azure Site Recovery replication policy.

## EXAMPLES

## PARAMETERS

### -Policy
Specifies the Site Recovery policy object.

```yaml
Type: ASRPolicy
Parameter Sets: (All)
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

[Get-AzureRmSiteRecoveryPolicy](./Get-AzureRmSiteRecoveryPolicy.md)

[New-AzureRmSiteRecoveryPolicy](./New-AzureRmSiteRecoveryPolicy.md)
