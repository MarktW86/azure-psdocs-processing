---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
ms.assetid: 31B92E0F-E46C-4371-8AC9-6C2B497C979B
online version:
schema: 2.0.0
updated_at: 04/25/2017 20:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/DuncanmaMSFT-patch-1/Azure%20AD%20Cmdlets/AzureAD/v2preview/Add-AzureADDeviceRegisteredOwner.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/DuncanmaMSFT-patch-1/Azure%20AD%20Cmdlets/AzureAD/v2preview/Add-AzureADDeviceRegisteredOwner.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/c5cc449ee6e2b805fc85a9e05130b06b10899f67
ms.topic: reference
ms.service: active-directory
---

# Add-AzureADDeviceRegisteredOwner

## SYNOPSIS
Adds a registered owner for a device.

## SYNTAX

```
Add-AzureADDeviceRegisteredOwner -ObjectId <String> -RefObjectId <String> [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureADDeviceRegisteredOwner** cmdlet adds a registerd owner for an Azure Active Directory device.

## EXAMPLES

## PARAMETERS

### -ObjectId
Specifies the object ID. 
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
Specifies the ID of the Active Directory object to add.
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

[Get-AzureADDeviceRegisteredOwner](./Get-AzureADDeviceRegisteredOwner.md)

[Remove-AzureADDeviceRegisteredOwner](./Remove-AzureADDeviceRegisteredOwner.md)
