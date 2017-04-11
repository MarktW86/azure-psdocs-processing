---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/11/2017 21:04 PM
ms.date: 04/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Get-AzureStackToken.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackAdmin/v0.10.6/Get-AzureStackToken.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/da0fd350a2a76c2d3edbf597f3826de129c926e5
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
---

# Get-AzureStackToken

## SYNOPSIS
The Get-AzureStackToken cmdlet gets a token to be used to make calls to Azurestack Resource Manager.
The cmdlet will be deprecated in a future release

## SYNTAX

### ADFS (Default)
```
Get-AzureStackToken [-Authority] <String> [-Resource <String>] [-ClientId <String>]
 [-Credential <PSCredential>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-PipelineVariable <String>] [<CommonParameters>]
```

### AAD
```
Get-AzureStackToken [-Authority] <String> -Resource <String> -AadTenantId <String> [-ClientId <String>]
 [-Credential <PSCredential>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-PipelineVariable <String>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-AzureStackToken -Authority $aadAuthorityEndpoint -AadTenantId $AadTenantId -Resource $aadResource -Credential (Get-Credential) -Verbose
```

Description

-----------

The following example gets the access token for the specified user
            $endpoints = Invoke-RestMethod -Method Get -Uri "$($ArmEndpoint.TrimEnd('/'))/metadata/endpoints?api-version=2015-01-01" -Verbose
            $aadAuthorityEndpoint = $endpoints.authentication.loginEndpoint
            $aadResource = $endpoints.authentication.audiences\[0\]

            Get-AzureStackToken -Authority $aadAuthorityEndpoint -AadTenantId $AadTenantId -Resource $aadResource -Credential (Get-Credential) -Verbose

## PARAMETERS

### -AadTenantId
Azure active directory(AAD) tenant Id of the user belonging to the  AAD tenant group

```yaml
Type: String
Parameter Sets: AAD
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Authority
Authority endpoint for authentication, typically of the form https://login.windows.net.
The value can be obtained by access the ARM metadata endpoint https://\<ArmUri\>/metadata/endpoints?api-version=2015-01-01 and reading the value of loginEndpoint

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClientId
The ClientId parameter is optional.
This parameter will be removed in a future release.
Please omit this

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

### -Credential
Specifies the credential for the user for whom we need the access token

```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
Not Specified

The following values are permitted for this object type.

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
Not Specified

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
Not Specified

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

### -Resource
Resource value for authentication, The value can be obtained by access the ARM metadata endpoint https://\<ArmUri\>/metadata/endpoints?api-version=2015-01-01 and reading the value of audiences

```yaml
Type: String
Parameter Sets: ADFS
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: AAD
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

### System.Object

## NOTES

## RELATED LINKS

