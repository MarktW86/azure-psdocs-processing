---
external help file: Microsoft.Open.MS.GraphBeta.PowerShell.dll-Help.xml
ms.assetid: 1E76B8D2-A7DF-49EE-8E22-6BFEE24A8B7F
online version:
schema: 2.0.0
updated_at: 05/26/2017 23:05 PM
ms.date: 05/26/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2preview/Add-AzureADApplicationPolicy.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2preview/Add-AzureADApplicationPolicy.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/ff946f6f9accc687a0d5bfca0f9070d9c3ef7642
ms.topic: reference
---

# Add-AzureADApplicationPolicy


## SYNOPSIS
**The Add-AzureADApplicationPolicy cmdlet is not available at this time**.

## SYNTAX

```
Add-AzureADApplicationPolicy -Id <String> -RefObjectId <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureADApplicationPolicy** cmdlet adds an Azure Active Directory application policy.

## EXAMPLES

### Example 1: Add an application policy
```
PS C:\>Add-AzureADApplicationPolicy -ObjectId <object id of application> -RefObjectId <object id of policy>
```

This command adds an application policy.

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

### -RefObjectId
Specifies the ID of the policy.

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

### -Id
The ID of the application for which you need to set the policy

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

[Get-AzureADApplicationPolicy](./Get-AzureADApplicationPolicy.md)

[Remove-AzureADApplicationPolicy](./Remove-AzureADApplicationPolicy.md)

