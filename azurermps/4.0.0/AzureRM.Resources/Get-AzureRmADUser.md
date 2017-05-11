---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
ms.assetid: BF254F2F-F658-45CC-8AC8-53FF96CFCAAD
online version:
schema: 2.0.0
updated_at: 05/11/2017 18:05 PM
ms.date: 05/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v4.0.0/Get-AzureRmADUser.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v4.0.0/Get-AzureRmADUser.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a9b160b3b332c6a38589f1828b17cf2391c2454e
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-resource-manager
---

# Get-AzureRmADUser

## SYNOPSIS
Filters active directory users.

## SYNTAX

### EmptyParameterSet (Default)
```
Get-AzureRmADUser [-UserPrincipalName <String>] [<CommonParameters>]
```

### SearchStringParameterSet
```
Get-AzureRmADUser -SearchString <String> [<CommonParameters>]
```

### ObjectIdParameterSet
```
Get-AzureRmADUser -ObjectId <Guid> [<CommonParameters>]
```

### UPNParameterSet
```
Get-AzureRmADUser -UserPrincipalName <String> [<CommonParameters>]
```

### MailParameterSet
```
Get-AzureRmADUser -Mail <String> [<CommonParameters>]
```

## DESCRIPTION
Filters active directory users.

## EXAMPLES

### --------------------------  Filters users using UPN  --------------------------
```
PS C:\> Get-AzureRmADUser -UPN foo@domain.com
```

Gets user with foo@domain.com

### --------------------------  Filters users using Search String  --------------------------
```
PS C:\> Get-AzureRmADUser -SearchString Joe
```

Filters all ad users that has Joe in the display name.

### --------------------------  List AD users  --------------------------
```
PS C:\> Get-AzureRmADUser
```

Gets all AD users

## PARAMETERS

### -Mail
```yaml
Type: String
Parameter Sets: MailParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ObjectId
Object id of the user.

```yaml
Type: Guid
Parameter Sets: ObjectIdParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SearchString
The user display name

```yaml
Type: String
Parameter Sets: SearchStringParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UserPrincipalName
UPN of the user.

```yaml
Type: String
Parameter Sets: EmptyParameterSet
Aliases: UPN

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: UPNParameterSet
Aliases: UPN

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureRmADUser]()

[Set-AzureRmADUser]()

[Remove-AzureRmADUser]()

