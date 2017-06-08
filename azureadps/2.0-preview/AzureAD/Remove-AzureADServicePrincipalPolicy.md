---
external help file: Microsoft.Open.MS.GraphBeta.PowerShell.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 06/08/2017 21:06 PM
ms.date: 06/08/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/rodejo5-10/Azure%20AD%20Cmdlets/AzureAD/v2preview/Remove-AzureADServicePrincipalPolicy.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/rodejo5-10/Azure%20AD%20Cmdlets/AzureAD/v2preview/Remove-AzureADServicePrincipalPolicy.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/d84c5a0765fd953cea9f2476361803b8c96211af
ms.topic: reference
---

# Remove-AzureADServicePrincipalPolicy

## SYNOPSIS

## SYNTAX

```
Remove-AzureADServicePrincipalPolicy -Id <String> -PolicyId <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>]
```

## DESCRIPTION

## EXAMPLES

### Example 1: Remove a service principal policy
```
PS C:\>Remove-AzureADApplicationPolicy -ObjectId <object id of application> -PolicyId <object id of policy>
```

This command removes a service principal policy.

## PARAMETERS

### -InformationAction
Specifies how this cmdlet responds to an information event.
The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

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
Specifies an information variable.

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

### -PolicyId
Specifies the object ID of a policy.

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
{{Fill Id Description}}

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

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureADServicePrincipalPolicy]()

[Get-AzureADServicePrincipalPolicy]()

