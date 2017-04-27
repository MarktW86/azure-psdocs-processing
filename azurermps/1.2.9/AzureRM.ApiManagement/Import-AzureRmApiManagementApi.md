---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/27/2017 22:04 PM
ms.date: 04/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Import-AzureRmApiManagementApi.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Import-AzureRmApiManagementApi.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a5140f27ab8f99c2992dc2ba0c9a1cd31941b109
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: api-Management
---

# Import-AzureRmApiManagementApi

## SYNOPSIS
Imports API from file or URL in one of the supported formats.

## SYNTAX

### From Local File (Default)
```
Import-AzureRmApiManagementApi -Context <PsApiManagementContext> [-ApiId <String>]
 -SpecificationFormat <PsApiManagementApiFormat> -SpecificationPath <String> [-Path <String>]
```

### From URL
```
Import-AzureRmApiManagementApi -Context <PsApiManagementContext> [-ApiId <String>]
 -SpecificationFormat <PsApiManagementApiFormat> -SpecificationUrl <String> [-Path <String>]
```

## DESCRIPTION
Imports API from file or URL in one of the supported formats (Wadl, Swagger).

## EXAMPLES

### --------------------------  Example 1  --------------------------
@{paragraph=PS C:\\\>}

```
Import-AzureRmApiManagementApi -Context $apimContext -SpecificationFormat 'Wadl' -SpecificationPath 'C:\contoso\specifications\echoapi.wadl' -Path 'apis'
```

Import API from WADL file.

### --------------------------  Example 2  --------------------------
@{paragraph=PS C:\\\>}

```
Import-AzureRmApiManagementApi -Context $apimContext -SpecificationFormat 'Swagger' -SpecificationPath 'C:\contoso\specifications\echoapi.swagger' -Path 'apis'
```

Import API from Swagger file.

### --------------------------  Example 3  --------------------------
@{paragraph=PS C:\\\>}

```
Import-AzureRmApiManagementApi -Context $apimContext -SpecificationFormat 'Wadl' -SpecificationUrl 'http://contoso.com/specifications/wadl/echoapi' -Path 'apis'
```

Import API from WADL link.

## PARAMETERS

### -Context
Instance of PsApiManagementContext.
This parameter is required.

```yaml
Type: PsApiManagementContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApiId
Identifier for importing API.
This parameter is optional.
If not specified the identifier will be generated.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SpecificationFormat
Specification format (Wadl, Swagger).
This parameter is required.

```yaml
Type: PsApiManagementApiFormat
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SpecificationPath
Specification file path.
This parameter is required.

```yaml
Type: String
Parameter Sets: From Local File
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
Web API Path.
Last part of the API's public URL.
This URL will be used by API consumers for sending requests to the web service.
Must be 1 to 400 characters long.
This parameter is optional.
Default value is $null.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SpecificationUrl
Specification URL.
This parameter is required.

```yaml
Type: String
Parameter Sets: From URL
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementApi
Imported API

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, api, apimanagement, apimgmt, apism

## RELATED LINKS

