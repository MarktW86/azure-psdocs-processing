---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=846353
schema: 2.0.0
ms.assetid: 5b4a72f5-2df1-4ae1-b020-a3d30f759a8b
updated_at: 04/21/2017 15:04 PM
ms.date: 04/21/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/AADRM/vlatest/Clear-AadrmDoNotTrackUserGroup.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/AADRM/vlatest/Clear-AadrmDoNotTrackUserGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/f34bcd754f9ec159ad5ec20f89432fa7fad4a9a6
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
ms.service: rights-management
---

# Clear-AadrmDoNotTrackUserGroup

## SYNOPSIS
Clears the group for the users who must not be tracked by Rights Management.

## SYNTAX

```
Clear-AadrmDoNotTrackUserGroup
```

## DESCRIPTION
The Clear-AadrmDoNotTrackUserGroup cmdlet removes the currently configured group for the users who must not be tracked by the Azure Rights Management document tracking feature. This configuration might be needed for privacy requirements. For more information, see [Privacy controls for your document tracking site](https://docs.microsoft.com/information-protection/rms-client/client-admin-guide-document-tracking#privacy-controls-for-your-document-tracking-site).

This cmdlet does not delete the specified group from Azure Active Directory. Instead, a group will no longer be used to exempt users from tracking. As a result, all users in your organization will now be tracked when you use the document tracking feature. 

You must use PowerShell to remove this group from the Azure Rights Management service; you cannot do this configuration by using a management portal.


## EXAMPLES

### Example 1
```
PS C:\>Clear-AadrmDoNotTrackUserGroup
```

This command removes the currently configured group (if set) that exempts users from being tracked by the document tracking feature. As a result, all users in your organization can be tracked when you use the document tracking feature.


## PARAMETERS

## INPUTS

### None


## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

[Disable-AadrmSuperUserFeature](./Disable-AadrmSuperUserFeature.md)

[Enable-AadrmDocumentTrackingFeature](./Enable-AadrmDocumentTrackingFeature.md)

[Get-AadrmDoNotTrackUserGroup](./Get-AadrmDoNotTrackUserGroup.md)

[Set-AadrmDoNotTrackUserGroup](./Set-AadrmDoNotTrackUserGroup.md)


