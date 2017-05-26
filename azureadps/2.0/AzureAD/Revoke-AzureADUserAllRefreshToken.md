---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/20/2017 04:04 AM
ms.date: 04/20/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-8/Azure%20AD%20Cmdlets/AzureAD/v2/Revoke-AzureADUserAllRefreshToken.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-8/Azure%20AD%20Cmdlets/AzureAD/v2/Revoke-AzureADUserAllRefreshToken.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/424c08eff259398d1aa2f26116c38cea5e911b45
ms.topic: reference
ms.service: active-directory
---

# Revoke-AzureADUserAllRefreshToken

## SYNOPSIS
Invalidates the refresh tokens issued to applications for a user. 

## SYNTAX

```
Revoke-AzureADUserAllRefreshToken -ObjectId <String> [<CommonParameters>]
```

## DESCRIPTION
The **Revoke-AzureADUserAllRefreshToken** cmdlet invalidates the refresh tokens issued to applications for a user. 
The cmdlet also invalidates tokens issued to session cookies in a browser for the user. 
The cmdlet operates by resetting the **refreshTokensValidFromDateTime** user property to the current date and time.

## EXAMPLES

### Example 1: Revoke refresh tokens for a user
```
PS C:\> Revoke-AzureADUserAllRefreshToken -ObjectId "a1d91a49-70c6-4d1d-a80a-b74c820a9a33"
```

This command revokes the tokens for the specified user. 

## PARAMETERS

### -ObjectId
Specifies the unique ID of a user. 

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

[Revoke-AzureADSignedInUserAllRefreshToken](./Revoke-AzureADSignedInUserAllRefreshToken.md)

[(#AzureAD: Certificate based authentication for iOS and Android now in preview!](https://blogs.technet.microsoft.com/enterprisemobility/2016/07/18/azuread-certificate-based-authentication-for-ios-and-android-now-in-preview/)
