---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
ms.assetid: CC6AF515-2F43-4E1B-BCBB-8DA23F3C6CBD
online version:
schema: 2.0.0
updated_at: 05/12/2017 22:05 PM
ms.date: 05/12/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71298/azureps-cmdlets-docs/ServiceManagement/Azure/v4.0.0/Get-AzureAutomationVariable.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71298/azureps-cmdlets-docs/ServiceManagement/Azure/v4.0.0/Get-AzureAutomationVariable.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/3b96c1e0b28fc56dfbf6de55728d5478e0d02def
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-asm
---

# Get-AzureAutomationVariable

## SYNOPSIS
Gets an Automation variable.

## SYNTAX

### ByAll (Default)
```
Get-AzureAutomationVariable -AutomationAccountName <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### ByName
```
Get-AzureAutomationVariable -Name <String> -AutomationAccountName <String> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureAutomationVariable** cmdlet gets one or more Microsoft Azure Automation variables.
By default, all variables are returned.
To get a specific variable, specify its name.

## EXAMPLES

### Example 1: Get a variable
```
PS C:\> $variable = Get-AzureAutomationVariable -AutomationAccountName
PS C:\> "Contoso17" -Name "MyVariable"
PS C:\> $value = $variable.value
```

These commands get an Automation variable called MyVariable and assign its value to a variable called $value.

## PARAMETERS

### -AutomationAccountName
Specifies the name of the Automation account.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of a variable.

```yaml
Type: String
Parameter Sets: ByName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.Automation.Model.Variable

## NOTES

## RELATED LINKS

[New-AzureAutomationVariable](./New-AzureAutomationVariable.md)

[Remove-AzureAutomationVariable](./Remove-AzureAutomationVariable.md)

[Set-AzureAutomationVariable](./Set-AzureAutomationVariable.md)


