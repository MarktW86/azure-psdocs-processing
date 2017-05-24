---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/24/2017 22:05 PM
ms.date: 05/24/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.1.3/Remove-AzureRmWebAppSSLBinding.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/anne2017/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.1.3/Remove-AzureRmWebAppSSLBinding.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/2d4a4fe807f8dce278c44747fc746934ed66d9fe
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: Websites
---

# Remove-AzureRmWebAppSSLBinding

## SYNOPSIS
Removes a secure socket layer (SSL) binding for a web app.

## SYNTAX

### S1
```
Remove-AzureRmWebAppSSLBinding [-Name] <String> [[-DeleteCertificate] <Boolean>] [-Force]
 [-ResourceGroupName] <String> [-WebAppName] <String> [[-Slot] <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### S2
```
Remove-AzureRmWebAppSSLBinding [-Name] <String> [[-DeleteCertificate] <Boolean>] [-Force] [-WebApp] <Site>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmWebAppSSLBinding** cmdlet removes a secure socket layer (SSL) binding for a web app that was built using the Web Apps feature of the Azure App Service.
An SSL binding associates a web app with a certificate.

## EXAMPLES

### Example 1: Remove an SSL binding for a web app and remove the certificate
```
Remove-AzureRmWebAppSSLBinding -ResourceGroupName "ContosoResourceGroup" -WebAppName "ContosoWebApp" -Name "www.contoso.com"
```

This example removes the SSL binding for the web app named "ContosoWebApp".
Because the **DeleteCertificate** parameter is not included, the certificate is deleted if it no longer has any SSL bindings.

### Example 2: Remove an SSL binding without removing the certificate
```
Remove-AzureRmWebAppSSLBinding -ResourceGroupName "ContosoResourceGroup" -WebAppName "ContosoWebApp" -Name "www.contoso.com" -DeleteCertificate $False
```

This example is similar to Example 1, but the certificate is not be deleted.

### Example 3: Use an object reference to remove an SSL binding
```
$myWebApp = Get-AzureRmWebApp -Name "ContosoWebApp"
Remove-AzureRmWebAppSSLBinding -WebApp $WebApp -Name "www.contoso.com"
```

This example uses an object to specify the web app for which you want to remove the SSL binding.
The **Get-AzureRmWebApp** cmdlet gets the web app named "ContosoWebApp" and stores the **WebApp** object in the **$myWebApp** variable.
The object is passed in the **WebApp** parameter of the **Remove-AzureRmWebAppSSLBinding** cmdlet to specify the web app that will have the binding removed.

## PARAMETERS

### -DeleteCertificate
Indicates whether to remove the certificate if the SSL binding being removed is the only binding used by the certificate.
If this parameter is set to **$False**, the certificate is not deleted when the binding is deleted.
If this parameter is set to **$True** or is not included in the command, the certificate is deleted along with the SSL binding if the certificate has no other bindings.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Indicates whether to forcefully remove the SSL binding.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the SSL binding to remove.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group to which the certificate is assigned. You cannot use the **ResourceGroupName** parameter and the **WebApp** parameter in the same command.

```yaml
Type: String
Parameter Sets: S1
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Slot
Specifies the name of the slot to which the web app is deployed.

```yaml
Type: String
Parameter Sets: S1
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebApp
Specifies a **WebApp** object that contains details about the web app.

```yaml
Type: Site
Parameter Sets: S2
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -WebAppName
Specifies the name of the web app for which this cmdlet removes an SSL binding. You cannot use the **WebAppName** parameter and the **WebApp** parameter in the same command.

```yaml
Type: String
Parameter Sets: S1
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Indicates whether to prompt the user for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Indicates whether to show what would happen if the cmdlet runs without actually running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

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

[Get-AzureRmWebAppSSLBinding](./Get-AzureRmWebAppSSLBinding.md)

[New-AzureRmWebAppSSLBinding](./New-AzureRmWebAppSSLBinding.md)

[Get-AzureRMWebAppSlot](./Get-AzureRMWebAppSlot.md)

[Get-AzureRmWebApp](./Get-AzureRmWebApp.md)
