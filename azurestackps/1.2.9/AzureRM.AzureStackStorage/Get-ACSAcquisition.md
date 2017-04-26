---
external help file: Microsoft.AzureStack.AzureConsistentStorage.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/26/2017 18:04 PM
ms.date: 04/26/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71305/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackStorage/v0.10.6/Get-ACSAcquisition.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71305/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackStorage/v0.10.6/Get-ACSAcquisition.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/51953647469adcc8031e9f92fbb62504cafc3aa8
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# Get-ACSAcquisition

## SYNOPSIS
Gets or lists acquisitions.

## SYNTAX

### GetAcquisitionSet
```
Get-ACSAcquisition [-ResourceGroupName] <String> [-FarmName] <String> -AcquisitionId <String>
 [[-SubscriptionId] <String>] [[-Token] <String>] [[-AdminUri] <Uri>] [-SkipCertificateValidation]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### ListAcquisitionSet
```
Get-ACSAcquisition [-ResourceGroupName] <String> [-FarmName] <String> [-TenantSubscriptionId <String>]
 [-StorageAccountName <String>] [-Container <String>] [[-SubscriptionId] <String>] [[-Token] <String>]
 [[-AdminUri] <Uri>] [-SkipCertificateValidation] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ACSAcquisition** gets or lists acquisitions by acquisition ID
This cmdlet lists acquisition by subscription, storage account, or Blob container.

## EXAMPLES

## PARAMETERS

### -AcquisitionId
Specifies the acquisition ID that this cmdlet gets.

```yaml
Type: String
Parameter Sets: GetAcquisitionSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -AdminUri


```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Container


```yaml
Type: String
Parameter Sets: ListAcquisitionSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FarmName
Specifies the name of the server farm.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

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

### -ResourceGroupName
Specifies the name of the resource group that contains the acquisition.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SkipCertificateValidation
Indicates that the cmdlet does not validate the certificate.

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

### -StorageAccountName
Specifies the name of the storage account that contains the acquisition.


```yaml
Type: String
Parameter Sets: ListAcquisitionSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubscriptionId
Specifies the ID of the subscription that contains the acquisition.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TenantSubscriptionId
Specifies the ID of the tenant subscription.

```yaml
Type: String
Parameter Sets: ListAcquisitionSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Token


```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.AzureStack.AzureConsistentStorage.Commands.FarmResponse

## OUTPUTS

### Microsoft.AzureStack.AzureConsistentStorage.Commands.AcquisitionResponse

## NOTES

## RELATED LINKS

[Remove-ACSAcquisition](./[Remove-ACSAcquisition.md)
