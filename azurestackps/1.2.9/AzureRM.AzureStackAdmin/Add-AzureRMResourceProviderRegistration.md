---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/25/2017 19:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Add-AzureRMResourceProviderRegistration.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Add-AzureRMResourceProviderRegistration.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/c4315559410058943d9b4bbae2b76e607f21de95
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# Add-AzureRMResourceProviderRegistration

## SYNOPSIS
Adds a resource provider manifest to the azure stack resource manager.

## SYNTAX

### MultipleExtensions (Default)
```
Add-AzureRMResourceProviderRegistration -Name <String> -Namespace <String> -ResourceGroup <String>
 -ArmLocation <String> -ResourceManagerType <ResourceManagerType> -DisplayName <String>
 -ProviderLocation <String> [-Extensions <String>] -ResourceTypes <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-PipelineVariable <String>]
 [<CommonParameters>]
```

### SingleExtension
```
Add-AzureRMResourceProviderRegistration -Name <String> -Namespace <String> -ResourceGroup <String>
 -ArmLocation <String> -ResourceManagerType <ResourceManagerType> -DisplayName <String>
 -ProviderLocation <String> -ExtensionName <String> -ExtensionUri <Uri> -ResourceTypes <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-PipelineVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureRMResourceProviderRegistration** cmdlet adds a resource provider manifest to the azure stack resource manager. This is needed to register any new resource provider with resource manager.

## EXAMPLES

### Example 1:
```
    # Make sure to provide the resource types json of the resource provider being registered
    $adminResourceTypesFile="$PSScriptRoot\AdminResourceTypes.json"
    $adminNamespace="Microsoft.Sql.Admin"
    $adminJson = Get-Content $adminResourceTypesFile -Raw | ConvertFrom-Json
    $adminJson | % { $_.endpoints\[0\].endpointUri="https://${VmName}:30010" }
    $adminJsonStr = $adminJson | ConvertTo-Json -Depth 4

    $location = "local"
    Add-AzureRMResourceProviderRegistration -Name $adminNamespace \`
    -Namespace $adminNamespace \`
    -ResourceGroup System \`
    -ArmLocation $location \`
    -ProviderLocation $location \`
    -DisplayName $adminNamespace \`
    -ExtensionName "SqlAdminExtension" \`
    -ExtensionUri "https://${VmName}:13002"  \`
    -ResourceManagerType Admin  \`
    -ResourceTypes $adminJsonStr
```

This example registers the resource provider manifest for a namespace.

## PARAMETERS

### -ArmLocation
{{Fill ArmLocation Description}}

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

### -DisplayName
Specifies the name to be displayed to the user for the resource provider manifest.

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

### -ExtensionName
Specifies the name of the extension that is associated with the resource provider manifest.

```yaml
Type: String
Parameter Sets: SingleExtension
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Extensions
Specifies a JSON string containing the names and URIs of the extensions that are associated with the resource provider manifest. This parameter is used only when there are multiple parameters associated with a single resource provider manifest.

```yaml
Type: String
Parameter Sets: MultipleExtensions
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExtensionUri
Specifies URI of the extension that is associated with the resource provider manifest.

```yaml
Type: Uri
Parameter Sets: SingleExtension
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

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
Specifies the name of the resource provider manifest.

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

### -Namespace
Specifies the namespace associated with the resource provider manifest.

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

### -ProviderLocation
Specifies the location of the resource provider.

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

### -ResourceGroup
Specifies the resource group under which the resource provider manifest is created.

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

### -ResourceManagerType
{{Fill ResourceManagerType Description}}

```yaml
Type: ResourceManagerType
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceTypes
Specifies the JSON string describing the resource provider manifest.

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

## OUTPUTS

### Microsoft.AzureStack.Management.Models.ProviderRegistrationModel

## NOTES

## RELATED LINKS
