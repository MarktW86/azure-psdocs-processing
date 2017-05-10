---
external help file: Microsoft.Azure.Commands.Profile.dll-Help.xml
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Profile/Commands.Profile/help/Save-AzureRmContext.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Profile/Commands.Profile/help/Save-AzureRmContext.md
gitcommit: https://github.com/Azure/azure-powershell/blob/63f2a98075c8f1cb88669fd63425db2a4d79107b
updated_at: 05/10/2017 17:05 PM
ms.date: 05/10/2017
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: subscription
---

# Save-AzureRmContext

## SYNOPSIS
Saves the current authentication information for use in other PowerShell sessions.

## SYNTAX

```
Save-AzureRmContext [[-Profile] <AzureRMProfile>] [-Path] <String> [-Force] [-WhatIf] [-Confirm]
```

## DESCRIPTION
The Save-AzureRmContext cmdlet saves the current authentication information for use in other PowerShell sessions.

## EXAMPLES

### Example 1: Saving the current session's context
```
PS C:\> Add-AzureRmAccount
PS C:\> Save-AzureRmContext -Path C:\test.json
```

This example saves the current session's Azure context to the JSON file provided.

### Example 2: Saving a given context
```
PS C:\> Save-AzureRmContext -Profile (Add-AzureRmAccount) -Path C:\test.json
```

This example saves the Azure context that is passed through to the cmdlet to the JSON file provided.

## PARAMETERS

### -Force
Overwrite the given file if it exists

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
Specifies the path of the file to which to save authentication information.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies the Azure context from which this cmdlet reads.
If you do not specify a context, this cmdlet reads from the local default context.

```yaml
Type: AzureRMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### Microsoft.Azure.Commands.Common.Authentication.Models.AzureRMProfile


## OUTPUTS

### Microsoft.Azure.Commands.Profile.Models.PSAzureProfile


## NOTES

## RELATED LINKS

