---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=846352
schema: 2.0.0
ms.assetid: a168cc5e-4e90-4a6d-8241-2f6d9dc27d7e
updated_at: 04/21/2017 15:04 PM
ms.date: 04/21/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/AADRM/vlatest/Set-AadrmDoNotTrackUserGroup.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/AADRM/vlatest/Set-AadrmDoNotTrackUserGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/f34bcd754f9ec159ad5ec20f89432fa7fad4a9a6
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
ms.service: rights-management
---

# Set-AadrmDoNotTrackUserGroup

## SYNOPSIS
Sets a group for the users who must not be tracked by Rights Management.

## SYNTAX

```
Set-AadrmDoNotTrackUserGroup -EmailAddress <String>
```

## DESCRIPTION
The Set-AadrmDoNotTrackUserGroup cmdlet sets a group for your Azure Rights Management service when you use document tracking and you have users who must not be tracked. This configuration might be needed for privacy requirements. For more information, see [Privacy controls for your document tracking site](https://docs.microsoft.com/information-protection/rms-client/client-admin-guide-document-tracking#privacy-controls-for-your-document-tracking-site).

If this cmdlet has been run before, running it again overwrites the group that was set previously. You can set only one group, but it can contain nested groups.

You must use PowerShell to set this group so that users are not tracked; you cannot do this configuration by using a management portal.

## EXAMPLES

### Example 1
```
PS C:\>Set-AadrmDoNotTrackUserGroup -GroupEmailAddress "DoNotTrackUserGroup@contoso.com"
```

This command sets a group that has the email address of DoNotTrackUserGroup@contoso.com for the Contoso organization so that users in that group will not be tracked with the document tracking feature.

## PARAMETERS

### -EmailAddress
Specifies the email address of the group whose members will be exempt from being tracked with the document tracking feature.

You can specify a group that contains individual users, or nested groups. The email address must be a valid group email address that already exists in the organization.


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

## INPUTS

### None


## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

[Clear-AadrmDoNotTrackUserGroup](./Clear-AadrmDoNotTrackUserGroup.md)

[Disable-AadrmSuperUserFeature](./Disable-AadrmSuperUserFeature.md)

[Enable-AadrmDocumentTrackingFeature](./Enable-AadrmDocumentTrackingFeature.md)

[Get-AadrmDoNotTrackUserGroup](./Get-AadrmDoNotTrackUserGroup.md)

