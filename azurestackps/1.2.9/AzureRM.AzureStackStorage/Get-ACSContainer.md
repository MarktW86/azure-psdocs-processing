---
external help file: Microsoft.AzureStack.AzureConsistentStorage.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/03/2017 00:05 AM
ms.date: 05/03/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/armsql/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackStorage/v0.10.6/Get-ACSContainer.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/armsql/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackStorage/v0.10.6/Get-ACSContainer.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/1b1f65c3c0d4679af027f9576236919af044769d
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-stack
---

# Get-ACSContainer

## SYNOPSIS
Gets the ACS container.

## SYNTAX

```
Get-ACSContainer [-ResourceGroupName] <String> [-FarmName] <String> [-ShareName] <String>
 [[-Intent] <ContainerGetIntent>] [[-Count] <UInt32>] [[-SubscriptionId] <String>] [[-Token] <String>]
 [[-AdminUri] <Uri>] [-SkipCertificateValidation] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ACSContainer** cmdlet gets the Azure Consistent Storage (ACS) container.

## EXAMPLES

## PARAMETERS

### -AdminUri
Specifies the link, as a URI, to the service administrator.

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

### -Count


```yaml
Type: UInt32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 7
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

### -Intent


```yaml
Type: ContainerGetIntent
Parameter Sets: (All)
Aliases: 
Accepted values: Migration

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that holds the ACS container.

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

### -ShareName
Specifies the name of the used in the Azure Consistent Storage system.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 5
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

### -SubscriptionId
Specifies the subscription ID. 

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

### System.String
System.Uri

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

[Get-ACSContainerMigrationStatus](./Get-ACSContainerMigrationStatus.md)
