---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/25/2017 19:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Set-AzureRMResourceProviderRegistration.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Set-AzureRMResourceProviderRegistration.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/c4315559410058943d9b4bbae2b76e607f21de95
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# Set-AzureRMResourceProviderRegistration

## SYNOPSIS
Updates the provider registration manifest with the new provider registration model.

## SYNTAX

```
Set-AzureRMResourceProviderRegistration -ProviderRegistration <ProviderRegistrationModel>
 -ResourceGroup <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-PipelineVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRMResourceProviderRegistration** cmdlet updates the provider registration manifest with the new provider registration model.

## EXAMPLES

### Example 1:
```
$manifest = Get-AzureRMResourceProviderRegistration -Name "Microsoft.Compute" -ResourceGroup "system" -Managed
Set-AzureRMResourceProviderRegistration -ProviderRegistration $manifest -ResourceGroup "System"
```

This example gets a **ProviderRegistrationModel** object, modifies the object, and then uses this object to update the provider registration manifest.

## PARAMETERS

### -InformationAction
Not specified.

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa
Accepted values: SilentlyContinue, Stop, Continue, Inquire

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Not specified.

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

### -PipelineVariable
Not specified.

```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProviderRegistration
Specifies an updated **ProviderRegistrationModel** object to be used for updating the existing provider registration data.

```yaml
Type: ProviderRegistrationModel
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ResourceGroup
Specifies the name of the resource group that contains the provider registration.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### Microsoft.AzureStack.Management.Models.ProviderRegistrationModel

## NOTES

## RELATED LINKS
