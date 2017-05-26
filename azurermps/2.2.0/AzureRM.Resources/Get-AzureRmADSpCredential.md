---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne052617/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Get-AzureRmADSpCredential.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne052617/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Get-AzureRmADSpCredential.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-resource-manager
---

# Get-AzureRmADSpCredential

## SYNOPSIS
Retrieves a list of credentials associated with a service principal.

## SYNTAX

### ObjectIdParameterSet (Default)
```
Get-AzureRmADSpCredential -ObjectId <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

### SPNParameterSet
```
Get-AzureRmADSpCredential -ServicePrincipalName <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The Get-AzureRmADSpCredential cmdlet can be used to retrieve a list of credentials associated with a service principal.
This command will retrieve all of the credential properties (but not the credential value) associated with the service principal.

## EXAMPLES

### --------------------------  Example 1  --------------------------
@{paragraph=PS C:\\\>}



```
PS E:\> Get-AzureRmADSpCredential -ServicePrincipalName http://test12345
```

Returns a list of credentials associated with the service principal having SPN 'http://test12345'.

## PARAMETERS

### -ObjectId
The object id of the service principal to retrieve credentials from.

```yaml
Type: String
Parameter Sets: ObjectIdParameterSet
Aliases: 

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

### -ServicePrincipalName
The name (SPN) of the service principal to retrieve credentials from.

```yaml
Type: String
Parameter Sets: SPNParameterSet
Aliases: 

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

[New-AzureRmADSpCredential]()

[Remove-AzureRmADSpCredential]()

[Get-AzureRmADServicePrincipal]()

