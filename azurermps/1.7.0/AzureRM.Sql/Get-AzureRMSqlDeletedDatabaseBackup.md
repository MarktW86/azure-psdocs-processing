---
external help file: Microsoft.Azure.Commands.Sql.dll-Help.xml
ms.assetid: C7772E32-C9F4-4F4E-9DB3-8A45DCCB6D14
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Sql/v1.0.12/Get-AzureRMSqlDeletedDatabaseBackup.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Sql/v1.0.12/Get-AzureRMSqlDeletedDatabaseBackup.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
---

# Get-AzureRmSqlDeletedDatabaseBackup

## SYNOPSIS
Gets a deleted database that you can restore.

## SYNTAX

```
Get-AzureRmSqlDeletedDatabaseBackup [-ServerName] <String> [[-DatabaseName] <String>]
 [[-DeletionDate] <DateTime>] [-ResourceGroupName] <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmSqlDeletedDatabaseBackup** cmdlet gets a specified deleted SQL database backup that you can restore, or all deleted backups that you can restore.

This cmdlet is also supported by the SQL Server Stretch Database service on Azure.

## EXAMPLES

### Example 1: Get all deleted database backups on a server
```
PS C:\>Get-AzureRmSqlDeletedDatabaseBackup -ResourceGroupName "ContosoResourceGroup" -ServerName "ContosoServer"
```

This command gets all deleted database backups on a server.

### Example 2: Get a specified deleted database backup
```
PS C:\>Get-AzureRmSqlDeletedDatabaseBackup -ResourceGroupName "ContosoResourceGroup" -ServerName "ContosoServer" -DatabaseName "ContosoDatabase"
```

This command gets the deleted database backup for ContosoDatabase.

## PARAMETERS

### -DatabaseName
Specifies the name of the database.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DeletionDate
Specifies the date, as a **DateTime** object, that the database was deleted.
To get a **DateTime** object, use the Get-Date cmdlet.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
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

### -ResourceGroupName
Specifies the name of the resource group to which the server is assigned.

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

### -ServerName
Specifies the name of the database server.

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

## NOTES

## RELATED LINKS

[Get-AzureRmSqlDatabase](./Get-AzureRmSqlDatabase.md)
