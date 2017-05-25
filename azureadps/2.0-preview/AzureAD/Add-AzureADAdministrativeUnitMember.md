---
external help file: Microsoft.Open.AzureADBeta.Graph.PowerShell.dll-Help.xml
ms.assetid: C2254A89-1700-4321-99FD-529E481705A3
online version:
schema: 2.0.0
updated_at: 04/25/2017 20:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/VinceSmith-patch-2/Azure%20AD%20Cmdlets/AzureAD/v2preview/Add-AzureADAdministrativeUnitMember.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/VinceSmith-patch-2/Azure%20AD%20Cmdlets/AzureAD/v2preview/Add-AzureADAdministrativeUnitMember.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/c5cc449ee6e2b805fc85a9e05130b06b10899f67
ms.topic: reference
ms.service: active-directory
---

# Add-AzureADAdministrativeUnitMember

## SYNOPSIS
Adds an administrative unit member.

## SYNTAX

```
Add-AzureADAdministrativeUnitMember -ObjectId <String> -RefObjectId <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureADAdministrativeUnitMember** cmdlet adds an Active Directory administrative unit member.

## EXAMPLES

## PARAMETERS

### -InformationAction
Specifies how this cmdlet responds to an information event.
The acceptable values for this parameter are:
* Continue
* Ignore
* Inquire
* SilentlyContinue
* Stop
* Suspend
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
Specifies a variable in which to store an information event message.
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

### -ObjectId
Specifies the ID of an Active Directory administrative unit.
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

### -RefObjectId
Specifies the unique ID of the specific Azure Active Directory object that will be assigned as owner/manager/member.
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

[Get-AzureADAdministrativeUnitMember](./Get-AzureADAdministrativeUnitMember.md)

[Remove-AzureADAdministrativeUnitMember](./Remove-AzureADAdministrativeUnitMember.md)
