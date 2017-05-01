---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400620
schema: 2.0.0
ms.assetid: C019DD8B-8C2C-487C-B730-38E50A170180
updated_at: 05/01/2017 16:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/AADRM/vlatest/Remove-AadrmRoleBasedAdministrator.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-doctracking/Azure%20Information%20Protection/AADRM/vlatest/Remove-AadrmRoleBasedAdministrator.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/64e9c474de8ba424ec88327ada5252d3a5907d98
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
ms.service: rights-management
---

# Remove-AadrmRoleBasedAdministrator

## SYNOPSIS
Removes administrative rights from Rights Management.

## SYNTAX

### ObjectId
```
Remove-AadrmRoleBasedAdministrator [-ObjectId <Guid>] [-Role <Role>] [<CommonParameters>]
```

### DisplayName
```
Remove-AadrmRoleBasedAdministrator [-SecurityGroupDisplayName <String>] [-Role <Role>] [<CommonParameters>]
```

### EmailAddress
```
Remove-AadrmRoleBasedAdministrator [-EmailAddress <String>] [-Role <Role>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AadrmRoleBasedAdministrator** cmdlet removes administrative rights to your organization's Azure Rights Management service, so that administrators you have previously delegated to configure this service can no longer do so by using PowerShell commands.

You must use PowerShell to configure delegated administrative control for the Azure Rights Management service; you cannot do this configuration by using a management portal.

To see the full list of delegated administrators for the Azure Rights Management service, use [Get-AadrmRoleBasedAdministrator](./Get-AadrmRoleBasedAdministrator.md). Run the Remove-AadrmRoleBasedAdministrator cmdlet for each user or group that you want to remove from the list. 

## EXAMPLES

### Example 1: Remove administrative rights by using a display name
```
PS C:\>Remove-AadrmRoleBasedAdministrator -SecurityGroupDisplayName "Finance Employees"
```

This command removes administrative rights to the Azure Rights Management service for the group that has a display name of "Finance Employees".

### Example 2: Remove administrative rights by using an email address
```
PS C:\>Remove-AadrmRoleBasedAdministrator -EmailAddress "EvanNarvaez@Contoso.com"
```

This command removes administrative rights to the Azure Rights Management service for the user who has an email address of "EvanNarvaez@Contoso.com".


## PARAMETERS

### -EmailAddress
Specifies the email address of a user or group to remove administrative rights for the Azure Rights Management service. If the user has no email address, specify the user's Universal Principal Name.

```yaml
Type: String
Parameter Sets: EmailAddress
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -ObjectId
Specifies the GUID of a user or group to remove administrative rights for the Azure Rights Management service.

```yaml
Type: Guid
Parameter Sets: ObjectId
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Role
Specifies a role. The cmdlet removes an administrator that belongs to the role that you specify.

The acceptable values for this parameter are:

- ConnectorAdministrator

- GlobalAdministrator

If you do not specify a role, the cmdlet removes the administrator from the GlobalAdministrator role.

```yaml
Type: Role
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -SecurityGroupDisplayName
Specifies the display name of a user or group that should no longer have administrative rights for the Azure Rights Management service.

```yaml
Type: String
Parameter Sets: DisplayName
Aliases:

Required: False
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

[Add-AadrmRoleBasedAdministrator](./Add-AadrmRoleBasedAdministrator.md)

[Get-AadrmRoleBasedAdministrator](./Get-AadrmRoleBasedAdministrator.md)
