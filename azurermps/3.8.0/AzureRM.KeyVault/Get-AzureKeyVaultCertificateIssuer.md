---
external help file: Microsoft.Azure.Commands.KeyVault.dll-Help.xml
ms.assetid: 5F856280-C561-47B5-AA96-27E34C86D604
online version:
schema: 2.0.0
updated_at: 04/07/2017 09:04 AM
ms.date: 04/07/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71305/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.8.0/Get-AzureKeyVaultCertificateIssuer.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71305/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.8.0/Get-AzureKeyVaultCertificateIssuer.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/195dcb690a30a5f2c0ecd5606483862547ef544a
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: key-vault
---

# Get-AzureKeyVaultCertificateIssuer

## SYNOPSIS
Gets a certificate issuer for a key vault.

## SYNTAX

### ByVaultName (Default)
```
Get-AzureKeyVaultCertificateIssuer [-VaultName] <String> [<CommonParameters>]
```

### ByName
```
Get-AzureKeyVaultCertificateIssuer [-VaultName] <String> [-Name] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureKeyVaultCertificateIssuer** cmdlet gets a specified certificate issuer or all certificate issuers for a key vault in Azure Key Vault.

## EXAMPLES

### Example 1: Get a certificate issuer
```
PS C:\>Get-AzureKeyVaultCertificateIssuer -VaultName "Contosokv01" -Name "TestIssuer01"
Name                : TestIssuer01
IssuerProvider      : Test
AccountId           : 555
ApiKey              : 
OrganizationDetails : Microsoft.Azure.Commands.KeyVault.Models.KeyVaultCertificateOrganizationDetails
```

This command gets the certificate issuer named TestIssuer01.

## PARAMETERS

### -Name
Specifies the name of the certificate issuer to get.

```yaml
Type: String
Parameter Sets: ByName
Aliases: IssuerName

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VaultName
Specifies the name of a key vault.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### List<Microsoft.Azure.Commands.KeyVault.Models.CertificateIssuerIdentityItem>, Microsoft.Azure.Commands.KeyVault.Models.KeyVaultCertificateIssuer

## NOTES

## RELATED LINKS

[Remove-AzureKeyVaultCertificateIssuer](./Remove-AzureKeyVaultCertificateIssuer.md)

[Set-AzureKeyVaultCertificateIssuer](./Set-AzureKeyVaultCertificateIssuer.md)

[Set-AzureKeyVaultCertificateIssuer]()

