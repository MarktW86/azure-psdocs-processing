---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: 73384750-6F54-4B7D-AD7D-BE53426132A4
online version:
schema: 2.0.0
updated_at: 05/19/2017 20:05 PM
ms.date: 05/19/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Invoke-ServiceFabricDecryptText.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Invoke-ServiceFabricDecryptText.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/8d4c81aabdfff50fd2bedea27942bd6899fa7bd1
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
---

# Invoke-ServiceFabricDecryptText

## SYNOPSIS
Decrypts the text encrypted by the [Invoke-ServiceFabricEncryptText](/.Invoke-ServiceFabricEncryptText.md) cmdlet.

## SYNTAX

```
Invoke-ServiceFabricDecryptText [-CipherText] <String> [-StoreLocation <StoreLocation>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Invoke-ServiceFabricDecryptText** cmdlet decrypts text that was encrypted by using the [Invoke-ServiceFabricEncryptText](./Invoke-ServiceFabricEncryptText.md) cmdlet for verification in Service Fabric.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

> [!NOTE]
> In order to decrypt the text, the caller of this cmdlet should have access to the private key of the certificate used to encrypt the text.

## EXAMPLES

### Example 1: Decrypt text
```
PS C:\windows\system32> $EncryptedText = Invoke-ServiceFabricEncryptText -Text "hello world" -CertThumbprint $Thumbprint
-CertStore -StoreLocation LocalMachine -StoreName My

PS C:\windows\system32> Invoke-ServiceFabricDecryptText -CipherText $EncryptedText -StoreLocation "LocalMachine"
hello world
```

The first command encrypts text using the **Invoke-ServiceFabricEncryptText** cmdlet and stores the result in the variable named $EncryptedText.

The second command decrypts the text stored in the $EncryptedText variable and saves it to the store location named LocalMachine.

## PARAMETERS

### -CipherText
Specifies the cipher text for the cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -StoreLocation
Specifies the location of a certificate store.
Valid values are:

- CurrentUser
- LocalMachine

```yaml
Type: StoreLocation
Parameter Sets: (All)
Aliases: 
Accepted values: CurrentUser, LocalMachine

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeoutSec
Specifies the time-out period, in seconds, for the operation.

```yaml
Type: Int32
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

### String
This cmdlet accepts a string of cipher text.

## OUTPUTS

### System.Object
This cmdlet returns decrypted text as a **String**.

## NOTES

## RELATED LINKS

[Invoke-ServiceFabricEncryptText](./Invoke-ServiceFabricEncryptText.md)

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)
