---
external help file: Microsoft.Azure.Commands.Sql.dll-Help.xml
ms.assetid: 7302D785-9DD0-4CC0-93C9-9A6EA60591CF
online version:
schema: 2.0.0
updated_at: 05/11/2017 01:05 AM
ms.date: 05/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/sdw-version-test/azureps-cmdlets-docs/ResourceManager/AzureRM.Sql/v2.7.0/Suspend-AzureRmSqlDatabase.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/sdw-version-test/azureps-cmdlets-docs/ResourceManager/AzureRM.Sql/v2.7.0/Suspend-AzureRmSqlDatabase.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/05e3e6af398c016caa52517268d3cee57da15cc4
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: sql-database
---

# Suspend-AzureRmSqlDatabase

## SYNOPSIS
Suspends a SQL Data Warehouse database.

## SYNTAX

```
Suspend-AzureRmSqlDatabase [-ServerName] <String> -DatabaseName <String> [-ResourceGroupName] <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The **Suspend-AzureRmSqlDatabase** cmdlet suspends an Azure SQL Data Warehouse database.

## EXAMPLES

### Example 1: Suspends an Azure SQL Data Warehouse database
```
PS C:\>Suspend-AzureRmSqlDatabase -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -DatabaseName "Database01"
```

This command suspends an active Azure SQL Data Warehouse database.

## PARAMETERS

### -ServerName
Specifies the name of the server which hosts the database.

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

### -DatabaseName
Specifies the name of the database that this cmdlet suspends.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
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
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

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

### Microsoft.Azure.Commands.Sql.Database.Model.AzureSqlDatabaseModel

## OUTPUTS

### Microsoft.Azure.Commands.Sql.Database.Model.AzureSqlDatabaseModel

## NOTES
* The **Suspend-AzureRmSqlDatabase** cmdlet works only on Azure SQL Data Warehouse databases. This operation is not supported on Azure SQL Database Basic, Standard and Premium editions.

## RELATED LINKS

[Get-AzureRmSqlDatabase](./Get-AzureRmSqlDatabase.md)

[New-AzureRmSqlDatabase](./New-AzureRmSqlDatabase.md)

[Remove-AzureRmSqlDatabase](./Remove-AzureRmSqlDatabase.md)

[Resume-AzureRmSqlDatabase](./Resume-AzureRmSqlDatabase.md)

[Set-AzureRmSqlDatabase](./Set-AzureRmSqlDatabase.md)




