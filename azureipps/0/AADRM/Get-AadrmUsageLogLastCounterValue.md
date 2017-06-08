---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400618
schema: 2.0.0
ms.assetid: BE5835E8-F97C-4F0E-8B2A-6698819D61CD
updated_at: 04/11/2017 05:04 AM
ms.date: 04/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-ipclient/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmUsageLogLastCounterValue.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-ipclient/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmUsageLogLastCounterValue.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/2047afa5f7c701b3cf7c3a822ab28ef22a7a6869
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
---

# Get-AadrmUsageLogLastCounterValue

## SYNOPSIS
Gets the last counter value for the usage log.

## SYNTAX

```
Get-AadrmUsageLogLastCounterValue [<CommonParameters>]
```

## DESCRIPTION
The **Get-AadrmUsageLogLastCounterValue** cmdlet gets the last counter value for the usage log.

You must use PowerShell to get this information; you cannot do this action by using a management portal.

This cmdlet should be used only if you have usage logs prior to the usage logging change in February 2016.
After this date, the only Windows PowerShell cmdlet that you need for Azure RMS usage logging is [Get-AadrmUserLog](./Get-AadrmUserLog.md).

For more information about usage logging, see [Logging and analyzing usage of the Azure Rights Management service](https://docs.microsoft.com/information-protection/deploy-use/log-analyze-usage).

## EXAMPLES

### Example 1: Get the last counter value
```
PS C:\>Get-AadrmUsageLogLastCounterValue
```

This command gets the last counter value for the usage log for your organization.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Enable-AadrmUsageLogFeature](./Enable-AadrmUsageLogFeature.md)

[Logging and analyzing usage of the Azure Rights Management service](https://docs.microsoft.com/information-protection/deploy-use/log-analyze-usage)
