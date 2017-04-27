---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/25/2017 19:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/4.0.0/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Get-AzureRMResourceProviderRegistration.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/4.0.0/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Get-AzureRMResourceProviderRegistration.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/c4315559410058943d9b4bbae2b76e607f21de95
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# Get-AzureRMResourceProviderRegistration

## SYNOPSIS
Gets the registration details of a resource provider.

## SYNTAX

```
Get-AzureRMResourceProviderRegistration [-Name <String>] -ResourceGroup <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-PipelineVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmResourceProviderRegistration** cmdlet gets the registration details of a resource provider.

## EXAMPLES

### Example 1:
```
$registration = Get-AzureRMResourceProviderRegistration -Name "Microsoft.Sql.Admin" -ResourceGroup "System"
```

This command gets the registration details for the "Microsoft.Sql.Admin" resource provider that was registered under the "System" resource group.

## PARAMETERS

### -InformationAction
Not Specified.

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
Not Specified.

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

### -Name
Specifies the name of the resource provider.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PipelineVariable
Not Specified.

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

### -ResourceGroup
Specifies the name of the resource group under which the resource provider was registered.

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
