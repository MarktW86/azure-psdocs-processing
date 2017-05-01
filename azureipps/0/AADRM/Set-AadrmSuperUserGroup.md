---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=722838
schema: 2.0.0
ms.assetid: 23E946A0-E6FC-4F8C-8F3B-352AD48CE426
updated_at: 05/01/2017 16:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Set-AadrmSuperUserGroup.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Set-AadrmSuperUserGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/64e9c474de8ba424ec88327ada5252d3a5907d98
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
ms.service: rights-management
---

# Set-AadrmSuperUserGroup

## SYNOPSIS
Sets the super user group for Rights Management.

## SYNTAX

```
Set-AadrmSuperUserGroup -GroupEmailAddress <String> [<CommonParameters>]
```

## DESCRIPTION
The **Set-AadrmSuperUserGroup** cmdlet specifies a group to use as the super user group for your Azure Rights Management service. Members of this group are then super users, which means they become a Rights Management owner for all content that is protected by your organization. These super users can decrypt this protected content and remove protection from it, even if an expiration date has been set and expired. Typically, this level of access is required for legal eDiscovery and by auditing teams.

You can specify any group that has an email address, but be aware that for performance reasons, group membership is cached. For information about group requirements, see [Preparing users and groups for Azure Information Protection](https://docs.microsoft.com/information-protection/plan-design/prepare).

If a super user group already exists, running this cmdlet overwrites it. This cmdlet does not affect users that are individually assigned as super users with the [Add-AadrmSuperUser](./Add-AadrmSuperUser.md) cmdlet.

An organization can have only one super user group in addition to multiple users who are assigned the privilege individually, but you can nest groups.

You must use PowerShell to configure super users; you cannot do this configuration by using a management portal.

For more information about super users, see [Configuring super users for Azure Rights Management and discovery services or data recovery](https://docs.microsoft.com/information-protection/deploy-use/configure-super-users).

## EXAMPLES

### Example 1: Set the super user group
```
PS C:\>Set-AadrmSuperUserGroup -GroupEmailAddress "SuperUserGroup@contoso.com"
```

This command sets the super user group for the organization to SuperUserGroup@contoso.com.

## PARAMETERS

### -GroupEmailAddress
Specifies the group email address for the super user group.

*GroupEmailAddress* can specify a group that contains individual users or other nested groups. It must be a valid group email address for an existing group in the organization.


```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AadrmSuperUser](./Add-AadrmSuperUser.md)

[Clear-AadrmSuperUserGroup](./Clear-AadrmSuperUserGroup.md)

[Get-AadrmSuperUserGroup](./Get-AadrmSuperUserGroup.md)
