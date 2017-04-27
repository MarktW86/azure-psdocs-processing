---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/27/2017 22:04 PM
ms.date: 04/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Get-AzureRmADUser.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Get-AzureRmADUser.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a5140f27ab8f99c2992dc2ba0c9a1cd31941b109
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
Get-AzureRmADUser [-UserPrincipalName <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### SearchStringParameterSet
```
Get-AzureRmADUser -SearchString <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### ObjectIdParameterSet
```
Get-AzureRmADUser -ObjectId <Guid> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### UPNParameterSet
```
Get-AzureRmADUser -UserPrincipalName <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

### MailParameterSet
```
Get-AzureRmADUser -Mail <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## DESCRIPTION
Filters active directory users.

## EXAMPLES

### --------------------------  Filters users using UPN  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\> Get-AzureRmADUser -UPN foo@domain.com
```

Gets user with foo@domain.com

### --------------------------  Filters users using Search String  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\> Get-AzureRmADUser -SearchString Joe
```

Filters all ad users that has Joe in the display name.

### --------------------------  List AD users  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\> Get-AzureRmADUser
```

Gets all AD users

## PARAMETERS

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

### -InformationAction
@{Text=}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

### -Mail
@{Text=}

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

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureRmADUser]()

[Set-AzureRmADUser]()

[Remove-AzureRmADUser]()

