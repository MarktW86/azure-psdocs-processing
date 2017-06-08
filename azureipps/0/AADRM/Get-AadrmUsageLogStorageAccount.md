---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400619
schema: 2.0.0
ms.assetid: A3A194BD-D7B2-417F-902D-33D40BB3B332
updated_at: 04/11/2017 05:04 AM
ms.date: 04/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmUsageLogStorageAccount.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Get-AadrmUsageLogStorageAccount.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/2047afa5f7c701b3cf7c3a822ab28ef22a7a6869
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
---

# Get-AadrmUsageLogStorageAccount

## SYNOPSIS
Gets the location for usage logs.

## SYNTAX

```
Get-AadrmUsageLogStorageAccount [<CommonParameters>]
```

## DESCRIPTION
The **Get-AadrmUsageLogStorageAccount** cmdlet gets the Azure storage location for usage logs for Azure Rights Management.

You must use PowerShell to get this information; you cannot do this action by using a management portal.

This cmdlet should be used only if you have usage logs prior to the usage logging change in February 2016.
After this date, the only Windows PowerShell cmdlet that you need for Azure RMS usage logging is the [Get-AadrmUserLog](./Get-AadrmUserLog.md) cmdlet.

For more information about usage logging, see [Logging and analyzing usage of the Azure Rights Management service](https://docs.microsoft.com/information-protection/deploy-use/log-analyze-usage).

## EXAMPLES

### Example 1: Get the log location
```
PS C:\>Get-AadrmUsageLogStorageAccount
```

This command gets the location for your usage logs.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AadrmUserLog](./Get-AadrmUserLog.md)

[Set-AadrmUsageLogStorageAccount](./Set-AadrmUsageLogStorageAccount.md)

[Logging and analyzing usage of the Azure Rights Management service](https://docs.microsoft.com/information-protection/deploy-use/log-analyze-usage)
