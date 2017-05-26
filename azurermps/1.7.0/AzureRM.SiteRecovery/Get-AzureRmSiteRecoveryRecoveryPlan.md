---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
ms.assetid: 5DA460AF-2DB1-4303-B9D9-C51FD9674E4B
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne052617/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v1.1.11/Get-AzureRmSiteRecoveryRecoveryPlan.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne052617/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v1.1.11/Get-AzureRmSiteRecoveryRecoveryPlan.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: site-recovery
---

# Get-AzureRmSiteRecoveryRecoveryPlan

## SYNOPSIS
Gets a recovery plan in Site Recovery.

## SYNTAX

### Default (Default)
```
Get-AzureRmSiteRecoveryRecoveryPlan [<CommonParameters>]
```

### ByName
```
Get-AzureRmSiteRecoveryRecoveryPlan -Name <String> [-Path <String>] [<CommonParameters>]
```

### ByFriendlyName
```
Get-AzureRmSiteRecoveryRecoveryPlan -FriendlyName <String> [-Path <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmSiteRecoveryRecoveryPlan** cmdlet gets a recovery plan in Azure Site Recovery.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -FriendlyName
Specifies the friendly name of the recovery plan that this cmdlet gets.

```yaml
Type: String
Parameter Sets: ByFriendlyName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the recovery plan that this cmdlet gets.

```yaml
Type: String
Parameter Sets: ByName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
Specifies the file path to which this cmdlet saves the recovery plan.

```yaml
Type: String
Parameter Sets: ByName, ByFriendlyName
Aliases: 

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

[New-AzureRmSiteRecoveryRecoveryPlan](./New-AzureRmSiteRecoveryRecoveryPlan.md)

[Remove-AzureRmSiteRecoveryRecoveryPlan](./Remove-AzureRmSiteRecoveryRecoveryPlan.md)

[Update-AzureRmSiteRecoveryRecoveryPlan](./Update-AzureRmSiteRecoveryRecoveryPlan.md)


