---
external help file: Microsoft.Azure.Commands.NotificationHubs.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: 3D47346F-DF7A-441E-8623-95A07CA98FB5
updated_at: 11/11/2016 23:11 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.NotificationHubs/v2.1.0/Remove-AzureRmNotificationHubsNamespaceAuthorizationRules.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.NotificationHubs/v2.1.0/Remove-AzureRmNotificationHubsNamespaceAuthorizationRules.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf
ms.topic: reference
---

# Remove-AzureRmNotificationHubsNamespaceAuthorizationRules

## SYNOPSIS
Removes an authorization rule from a notification hub namespace.

## SYNTAX

```
Remove-AzureRmNotificationHubsNamespaceAuthorizationRules [-ResourceGroup] <String> [-Namespace] <String>
 [-AuthorizationRule] <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmNotificationHubsNamespaceAuthorizationRules** cmdlet removes a Shared Access Signature (SAS) authorization rule from a notification hub namespace.

Authorization rules manage access to a namespace.
This is done by through the creation of links, as URIs, based on different permission levels.
Permission levels can be of the following: 

- Listen
- Send
- Manage

Clients are directed to one of these URIs based on the appropriate permission level.
For instance, a client given the Listen permission is directed to the URI for that permission.

Removing an authorization rule also removes the corresponding user permission.

## EXAMPLES

### Example 1: Remove an authorization rule from a namespace
```
PS C:\>Remove-AzureRmNotificationHubNamespaceAuthorizationRules -Namespace "ContosoNamespace" -ResourceGroup "ContosoNotificationsGroup" -AuthorizationRule "ListenRule"
```

This command removes the authorization rule named ListenRule from the namespace named ContosoNamespace.
When you run this command you must specify the resource group that the namespace is assigned to.

## PARAMETERS

### -ResourceGroup
Specifies the resource group to which the namespace is assigned.
Resource groups organize items such as namespaces, notification hubs, and authorization rules in ways that help simply inventory management and Azure administration.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Namespace
Specifies the namespace to which the authorization rules are assigned.
Namespaces provide a way to group and categorize notification hubs.

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

### -AuthorizationRule
Specifies the name of the SAS authentication rule to be removed.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmNotificationHubsNamespaceAuthorizationRules](./Get-AzureRmNotificationHubsNamespaceAuthorizationRules.md)

[New-AzureRmNotificationHubsNamespaceAuthorizationRules](./New-AzureRmNotificationHubsNamespaceAuthorizationRules.md)

[Set-AzureRmNotificationHubsNamespaceAuthorizationRules](./Set-AzureRmNotificationHubsNamespaceAuthorizationRules.md)


