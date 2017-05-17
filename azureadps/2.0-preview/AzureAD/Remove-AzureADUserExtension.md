---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.Custom.dll-Help.xml
ms.assetid: 2D1768D6-29D4-4985-ADD3-8308FF370DDC
online version:
schema: 2.0.0
updated_at: 04/25/2017 20:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-5/Azure%20AD%20Cmdlets/AzureAD/v2preview/Remove-AzureADUserExtension.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-5/Azure%20AD%20Cmdlets/AzureAD/v2preview/Remove-AzureADUserExtension.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/c5cc449ee6e2b805fc85a9e05130b06b10899f67
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
ms.service: active-directory
---

# Remove-AzureADUserExtension

## SYNOPSIS
Removes a user extension.

## SYNTAX

### SetSingle
```
Remove-AzureADUserExtension -ObjectId <String> -ExtensionName <String> [<CommonParameters>]
```

### SetMultiple
```
Remove-AzureADUserExtension -ObjectId <String>
 -ExtensionNames <System.Collections.Generic.List`1[System.String]> [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureADUserExtension** cmdlet removes a user extension from Azure Active Directory (AD).

## EXAMPLES

## PARAMETERS

### -ExtensionName
Specifies the name of an extension.
```yaml
Type: String
Parameter Sets: SetSingle
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -ExtensionNames
Specifies an array of extension names.
```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: SetMultiple
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -ObjectId
Specifies an object ID.
```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureADUserExtension](./Get-AzureADUserExtension.md)

[Set-AzureADUserExtension](./Set-AzureADUserExtension.md)
