---
external help file: Microsoft.AzureStack.AzureConsistentStorage.Commands.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/03/2017 00:05 AM
ms.date: 05/03/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/4.1.0/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackStorage/v0.10.6/Start-ACSContainerMigration.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/4.1.0/azureps-cmdlets-docs/AzureStack/AzureRM.AzureStackStorage/v0.10.6/Start-ACSContainerMigration.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/1b1f65c3c0d4679af027f9576236919af044769d
ms.topic: reference
---

# Start-ACSContainerMigration

## SYNOPSIS
Starts the ACS container migration.

## SYNTAX

```
Start-ACSContainerMigration [-ResourceGroupName] <String> [-FarmName] <String>
 [-ContainerToMigrate] <Container> [-DestinationShareUncPath] <String> [[-SubscriptionId] <String>]
 [[-Token] <String>] [[-AdminUri] <Uri>] [-SkipCertificateValidation] [<CommonParameters>]
```

## DESCRIPTION
The **Start-ACSContainerMigration** cmdlet starts the Azure Consistent Storage (ACS) container migration.

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

### -ContainerToMigrate
Specifies the ACS container that this cmdlet migrates.

```yaml
Type: Container
Parameter Sets: (All)
Aliases: 

Required: True
Position: 5
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DestinationShareUncPath


```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 6
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -FarmName
Specifies the name of the ACS farm.

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

### -ResourceGroupName
Specifies the name of the resource group that contains the ACS farm.

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
Microsoft.AzureStack.AzureConsistentStorage.Models.Container
System.Uri

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

[Stop-ACSContainerMigration](./Stop-ACSContainerMigration.md)
