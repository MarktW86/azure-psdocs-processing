---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400614
schema: 2.0.0
ms.assetid: 508FBF5B-A405-4FCB-9EB3-39183F46F60A
updated_at: 04/17/2017 16:04 PM
ms.date: 04/17/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-ipclient/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmSuperUser.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-ipclient/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmSuperUser.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/5af92e98a02d763b2ab8dd55a422ee6800025892
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
---

# Get-AadrmSuperUser

## SYNOPSIS
Gets the super users for Rights Management.

## SYNTAX

```
Get-AadrmSuperUser [<CommonParameters>]
```

## DESCRIPTION
The **Get-AadrmSuperUser** cmdlet gets the super users for Azure Rights Management, who can unprotect or protect files for your organization when the super user feature is enabled by using the [Enable-AadrmSuperUserFeature](./Enable-AadrmSuperUserFeature.md) cmdlet.

You must use PowerShell to configure super users; you cannot do this configuration by using a management portal.

For more information about super users, see [Configuring super users for Azure Rights Management and discovery services or data recovery](https://docs.microsoft.com/information-protection/deploy-use/configure-super-users).

## EXAMPLES

### Example 1: List super users
```
PS C:\>Get-AadrmSuperUser
```

This command lists the super users for Rights Management.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AadrmSuperUser](./Add-AadrmSuperUser.md)

[Remove-AadrmSuperUser](./Remove-AadrmSuperUser.md)

[Enable-AadrmSuperUserFeature](./Enable-AadrmSuperUserFeature.md)

[Configuring super users for Azure Rights Management and discovery services or data recovery](https://docs.microsoft.com/information-protection/deploy-use/configure-super-users)
