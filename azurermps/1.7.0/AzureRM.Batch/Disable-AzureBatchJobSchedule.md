---
external help file: Microsoft.Azure.Commands.Batch.dll-Help.xml
ms.assetid: F5C53916-358D-43EF-813A-2C07ACA69FD3
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71298/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v1.1.4/Disable-AzureBatchJobSchedule.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/Graham71298/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v1.1.4/Disable-AzureBatchJobSchedule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: batch
---

# Disable-AzureBatchJobSchedule

## SYNOPSIS
Disables a Batch job schedule.

## SYNTAX

```
Disable-AzureBatchJobSchedule [-Id] <String> -BatchContext <BatchAccountContext> [<CommonParameters>]
```

## DESCRIPTION
The **Disable-AzureBatchJobSchedule** cmdlet disables an Azure Batch job schedule.
If you disable a schedule, jobs are not created according to that schedule.
You can enable a disabled schedule later.

## EXAMPLES

### Example 1: Disable a job schedule
```
PS C:\>Disable-AzureBatchJobSchedule -Id "JobSchedule17" -BatchContext $Context
```

This command disables the job schedule that has the ID JobSchedule17.
Use the **Get-AzureRmBatchAccountKeys** cmdlet to assign a context to the $Context variable.

## PARAMETERS

### -BatchContext
Specifies the **BatchAccountContext** instance that this cmdlet uses to interact with the Batch service.
To obtain a **BatchAccountContext** object that contains access keys for your subscription, use the Get-AzureRmBatchAccountKeys cmdlet.

```yaml
Type: BatchAccountContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Id
Specifies the ID of the job schedule that this cmdlet disables.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
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

[Enable-AzureBatchJobSchedule](./Enable-AzureBatchJobSchedule.md)

[Get-AzureRmBatchAccountKeys](./Get-AzureRmBatchAccountKeys.md)

[Get-AzureBatchJobSchedule](./Get-AzureBatchJobSchedule.md)

[New-AzureBatchJobSchedule](./New-AzureBatchJobSchedule.md)

[Remove-AzureBatchJobSchedule](./Remove-AzureBatchJobSchedule.md)

[Stop-AzureBatchJobSchedule](./Stop-AzureBatchJobSchedule.md)

[Azure Batch Cmdlets](./AzureRM.Batch.md)


