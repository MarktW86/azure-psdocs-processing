---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
ms.assetid: BDEA3F9D-AC23-402D-BA1F-AC617C7480A1
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/v3.8.0-April2017/src/ResourceManager/SiteRecovery/Commands.SiteRecovery/help/Remove-AzureRmSiteRecoveryNetworkMapping.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/v3.8.0-April2017/src/ResourceManager/SiteRecovery/Commands.SiteRecovery/help/Remove-AzureRmSiteRecoveryNetworkMapping.md
gitcommit: https://github.com/Azure/azure-powershell/blob/94e42834e29c78cafba9e3f1e99e14af92561036
updated_at: 04/26/2017 07:04 AM
ms.date: 04/26/2017
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: site-recovery
---

# Remove-AzureRmSiteRecoveryNetworkMapping

## SYNOPSIS
Removes a network mapping from the current Site Recovery vault.

## SYNTAX

```
Remove-AzureRmSiteRecoveryNetworkMapping -NetworkMapping <ASRNetworkMapping> [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRMSiteRecoveryNetworkMapping** cmdlet removes a network mapping from the current Azure Site Recovery vault.

## EXAMPLES

## PARAMETERS

### -NetworkMapping
Specifies the network mapping object.

```yaml
Type: ASRNetworkMapping
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

[Get-AzureRmSiteRecoveryNetworkMapping](./Get-AzureRmSiteRecoveryNetworkMapping.md)

[New-AzureRmSiteRecoveryNetworkMapping](./New-AzureRmSiteRecoveryNetworkMapping.md)
