---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/25/2017 20:04 PM
ms.date: 04/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/VinceSmith-patch-3/Azure%20AD%20Cmdlets/AzureAD/v2preview/Get-AzureADUserLicenseDetail.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/VinceSmith-patch-3/Azure%20AD%20Cmdlets/AzureAD/v2preview/Get-AzureADUserLicenseDetail.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/c5cc449ee6e2b805fc85a9e05130b06b10899f67
ms.topic: reference
ms.service: active-directory
---

# Get-AzureADUserLicenseDetail

## SYNOPSIS
Retrieves license details for a user

## SYNTAX

```
Get-AzureADUserLicenseDetail -ObjectId <String> [<CommonParameters>]
```

## DESCRIPTION
THis cmdlet retrieves license details for a user

## EXAMPLES

### Example 1
```
PS C:\WINDOWS\system32> Get-AzureADUserLicenseDetail -ObjectId df19e8e6-2ad7-453e-87f5-037f6529ae16

ObjectId                                    ServicePlans
--------                                    ------------
Hv-1hQIEDECePA-ellMl0cjsRfKvdY5Pth8n2BFN5fM {class ServicePlanInfo {...
Hv-1hQIEDECePA-ellMl0QQrjQe98RFBu9S0sbNUzvQ {class ServicePlanInfo {...
```

This example retrieves the license details of the user specified through the ObjectId parameter

## PARAMETERS

### -ObjectId
The object ID of the user for which the license details are retrieved

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

### System.String

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

