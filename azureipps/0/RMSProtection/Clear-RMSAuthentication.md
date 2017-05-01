---
external help file: AIP.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=734985
schema: 2.0.0
ms.assetid: D0D6B294-8664-4E9A-8553-5031F452CC64
updated_at: 02/08/2017 18:02 PM
ms.date: 02/08/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/RMSProtection/vlatest/Clear-RMSAuthentication.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/RMSProtection/vlatest/Clear-RMSAuthentication.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/b5b814c02caa6cd576a3db614749957f10782144
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
ms.service: rights-management
---

# Clear-RMSAuthentication

## SYNOPSIS
Clears credentials for a user who is authenticated to the Azure RMS service.

## SYNTAX

```
Clear-RMSAuthentication [<CommonParameters>]
```

## DESCRIPTION
The **Clear-RMSAuthentication** cmdlet clears the credentials that are used when a user has previously entered their user name and password to authenticate to Azure Rights Management (Azure RMS).

When you enter a user name and password to sign in to Azure RMS, the credentials are cached on the computer. Because these cached credentials are used across PowerShell sessions, to sign in as a different user, you must first run **Clear-RMSAuthentication**. You are then prompted for new credentials.

This cmdlet applies to Azure RMS only and when you authenticate as a user rather than a service principal. It does not apply to AD RMS.

Note: If you want to clear the credentials for a service principal that you specified with [Set-RMSServerAuthentication](./Set-RMSServerAuthentication), close your PowerShell session and start a new session that runs **Set-RMSServerAuthentication** with the new credentials.

## EXAMPLES

### Example 1: Clear authentication credentials
```
PS C:\>Clear-RMSAuthentication                        
Authentication cleared
```

This command clears the currently cached authentication credentials for a user who is authenticated to Azure RMS on a computer that is not joined to a domain.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Set-RMSServerAuthentication](./Set-RMSServerAuthentication.md)
