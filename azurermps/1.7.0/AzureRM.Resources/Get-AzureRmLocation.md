---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/02/2017 17:05 PM
ms.date: 05/02/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/Get-AzureRmLocation.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/Get-AzureRmLocation.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/fdff926f5dd35f9020f210f87b450464ba162edc
ms.topic: reference
ms.service: azure-resource-manager
---

# Get-AzureRmLocation

## SYNOPSIS

## SYNTAX

```
Get-AzureRmLocation [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

## DESCRIPTION
Get all locations and the supported resource providers.

If you find an issue with this cmdlet, please create an issue on https://github.com/Azure/azure-powershell/issues, with a lable "ResourceManager".

## EXAMPLES

### --------------------------  Example 1: Get all locations and the supported resource providers --------------------------
@{paragraph=PS C:\\\>}



```
PS C:\>Get-AzureRmLocation
```

This command gets all locations and the supported resource providers.

## PARAMETERS

### -ApiVersion
When set, indicates the version of the resource provider API to use.
If not specified, the API version is automatically determined as the latest available.

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

### -Pre
When set, indicates that the cmdlet should use pre-release API versions when automatically determining which version to use.

```yaml
Type: SwitchParameter
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

## NOTES

## RELATED LINKS

