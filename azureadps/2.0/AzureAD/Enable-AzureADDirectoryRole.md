---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
ms.assetid: 3719960D-7A77-414E-A20C-812B527F27AB
online version:
schema: 2.0.0
updated_at: 05/25/2017 18:05 PM
ms.date: 05/25/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/VinceSmith-patch-5/Azure%20AD%20Cmdlets/AzureAD/v2/Enable-AzureADDirectoryRole.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/VinceSmith-patch-5/Azure%20AD%20Cmdlets/AzureAD/v2/Enable-AzureADDirectoryRole.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/88b1e63fc06924cfafb7ea64a389bfca7d70c1cb
ms.topic: reference
ms.service: active-directory
---

# Enable-AzureADDirectoryRole

## SYNOPSIS
Activates an existing directory role in Azure Active Directory.

## SYNTAX

```
Enable-AzureADDirectoryRole [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-DirectoryRole <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Enable-AzureADDirectoryRole** cmdlet activates an existing directory role in Azure Active Directory.

## EXAMPLES

### Example 1: Enable a directory role
```
# Get Guest Inviter directory role template
$roleTemplate = Get-AzureADDirectoryRoleTemplate | ? { $_.DisplayName -eq "Guest Inviter" }

# Instantiate new DirectoryRole object
$newRole = New-Object -TypeName "Microsoft.Open.AzureAD.Model.DirectoryRole"

# Set templateId for role temaplate object to Guest Inviter objectId
$newRole.RoleTemplateId = $roleTemplate.ObjectId

# Enable an instance of the DirectoryRole template
Enable-AzureADDirectoryRole -DirectoryRole $newRole

```

The first command gets an inviter role that has the display name Guest Inviter by using the [Get-AzureADDirectoryRoleTemplate](./Get-AzureADDirectoryRoleTemplate.md) cmdlet. 
The command stores Guest Inviter in the $roleTemplate variable. 

The second command instantiates a new DirectoryRole object and stores it in $newRole.

The third command sets the role template Id for $newRole to the guest inviter role template Id.

The final command enables the directory role in $newRole.

## PARAMETERS

### -InformationAction
Specifies how this cmdlet responds to an information event. The acceptable values for this parameter are:

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
Specifies a variable in which to store an information event message.

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

### -RoleTemplateId
The ID of the Role template to enable

```yaml
Type: String
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

[Get-AzureADDirectoryRole](./Get-AzureADDirectoryRole.md)

[Get-AzureADDirectoryRoleTemplate](./Get-AzureADDirectoryRoleTemplate.md)
