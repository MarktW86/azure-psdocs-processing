---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400622
schema: 2.0.0
ms.assetid: ECE82C74-2902-475D-9DCE-6E9F3842024D
updated_at: 04/17/2017 16:04 PM
ms.date: 04/17/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/AADRM/vlatest/Set-AadrmMigrationUrl.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/AADRM/vlatest/Set-AadrmMigrationUrl.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/5af92e98a02d763b2ab8dd55a422ee6800025892
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
ms.service: rights-management
---

# Set-AadrmMigrationUrl

## SYNOPSIS
Sets the migration URL for Rights Management.

## SYNTAX

```
Set-AadrmMigrationUrl -Domain <String> [-Force] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AadrmMigrationUrl** cmdlet sets the migration URL for Azure Rights Management.

You must use PowerShell to set the migration URL; you cannot do this action by using a management portal.

Migration URLs let you migrate from Azure Rights Management to a supported on-premises Rights Management server. Use this migration technique if you need indefinite access to content that has been previously protected by using Azure Rights Management and you have decided to no longer use Azure Rights Management.

In addition to setting this migration URL for clients, you must export your keys and policies from the cloud service in the form of a trusted publishing domain (TPD file) and import them into an on-premises Rights Management server. For more information, see the instructions for exporting your tenant key in [Microsoft-managed: Tenant key lifecycle operations](https://docs.microsoft.com/information-protection/deploy-use/operations-microsoft-managed-tenant-key).

## EXAMPLES

### Example 1: Set a migration URL
```
PS C:\>Set-AadrmMigrationUrl -Domain "aadrm.online.contoso.com"
```

This command sets a migration URL for Rights Management.

## PARAMETERS

### -Domain
Specifies a URL for the domain to migrate.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Indicates that the cmdlet sets the value of the migration URL even if there is an existing migration URL.

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

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs. The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AadrmMigrationUrl](./Get-AadrmMigrationUrl.md)

[Microsoft-managed: Tenant key lifecycle operations](https://docs.microsoft.com/information-protection/deploy-use/operations-microsoft-managed-tenant-key)
