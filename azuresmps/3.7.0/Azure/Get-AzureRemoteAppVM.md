---
external help file: Microsoft.WindowsAzure.Commands.RemoteApp.dll-Help.xml
ms.assetid: D40937C2-9BF7-4371-A64C-B44F5B6B895E
online version:
schema: 2.0.0
updated_at: 03/29/2017 02:03 AM
ms.date: 03/29/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure/v3.7.0/Get-AzureRemoteAppVM.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure/v3.7.0/Get-AzureRemoteAppVM.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/828e5b8648af6bdf3119ffe0cd409647f00de183
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: false
---

# Get-AzureRemoteAppVM

## SYNOPSIS
Gets the virtual machines in an Azure RemoteApp collection.

## SYNTAX

```
Get-AzureRemoteAppVM -CollectionName <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRemoteAppVM** cmdlet gets the virtual machines created under an Azure RemoteApp collection for session hosting.

## EXAMPLES

### Example 1: Display the virtual machines in a collection
```
PS C:\> Get-AzureRemoteAppVM -CollectionName "Contoso"
```

This command displays the virtual machines used for session hosting in an Azure RemoteApp collection named Contoso.

## PARAMETERS

### -CollectionName
Specifies the name of the Azure RemoteApp collection.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

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

## NOTES

## RELATED LINKS

[Restart-AzureRemoteAppVM](./Restart-AzureRemoteAppVM.md)

