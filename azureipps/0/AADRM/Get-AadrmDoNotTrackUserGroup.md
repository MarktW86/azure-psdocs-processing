---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=846355
schema: 2.0.0
ms.assetid: 176a6f8e-258b-4bb9-8690-dd1bae05530c
updated_at: 04/21/2017 15:04 PM
ms.date: 04/21/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmDoNotTrackUserGroup.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmDoNotTrackUserGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/f34bcd754f9ec159ad5ec20f89432fa7fad4a9a6
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
ms.service: rights-management
---

# Get-AadrmDoNotTrackUserGroup

## SYNOPSIS
Gets the group for the users who must not be tracked by Rights Management.

## SYNTAX

```
Get-AadrmDoNotTrackUserGroup
```

## DESCRIPTION
The Get-AadrmDoNotTrackUserGroup cmdlet gets the email address of the currently configured group for the users who must not be tracked by the Azure Rights Management document tracking feature. 

This configuration might be needed for privacy requirements. For more information, see [Privacy controls for your document tracking site](https://docs.microsoft.com/information-protection/rms-client/client-admin-guide-document-tracking#privacy-controls-for-your-document-tracking-site).

You must use PowerShell to retrieve this information; you cannot see it by using a management portal. 

## EXAMPLES

### Example 1
```
PS C:\>Get-AadrmDoNotTrackUserGroup
```

This command gets the email address of the currently configured group for the users who will not be tracked with the document tracking feature.

## PARAMETERS

## INPUTS

### None


## OUTPUTS

### System.String
This operation returns the group email address as a **String**. If a group has not been configured, an empty **String** is returned.

## NOTES

## RELATED LINKS

[Clear-AadrmDoNotTrackUserGroup](./Clear-AadrmDoNotTrackUserGroup.md)

[Disable-AadrmSuperUserFeature](./Disable-AadrmSuperUserFeature.md)

[Enable-AadrmDocumentTrackingFeature](./Enable-AadrmDocumentTrackingFeature.md)

[Set-AadrmDoNotTrackUserGroup](./Set-AadrmDoNotTrackUserGroup.md)
