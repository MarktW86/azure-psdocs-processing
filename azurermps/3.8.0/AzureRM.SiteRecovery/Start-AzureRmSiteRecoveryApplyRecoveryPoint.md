---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
ms.assetid: 86A60FD6-551A-4A6B-A4D1-466F33CE714A
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/SiteRecovery/Commands.SiteRecovery/help/Start-AzureRmSiteRecoveryApplyRecoveryPoint.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/SiteRecovery/Commands.SiteRecovery/help/Start-AzureRmSiteRecoveryApplyRecoveryPoint.md
gitcommit: https://github.com/Azure/azure-powershell/blob/94e42834e29c78cafba9e3f1e99e14af92561036
updated_at: 04/28/2017 07:04 AM
ms.date: 04/28/2017
ms.topic: reference
---

# Start-AzureRmSiteRecoveryApplyRecoveryPoint

## SYNOPSIS
Changes a recovery point for a failed over protected item before commiting the failover operation.

## SYNTAX

```
Start-AzureRmSiteRecoveryApplyRecoveryPoint -RecoveryPoint <ASRRecoveryPoint>
 -ReplicationProtectedItem <ASRReplicationProtectedItem> [-DataEncryptionPrimaryCertFile <String>]
 [-DataEncryptionSecondaryCertFile <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Start-AzureRmSiteRecoveryApplyRecoveryPoint** changes a recovery point for a failed over protected item before it commits the failover operation.

## EXAMPLES

## PARAMETERS

### -RecoveryPoint
Specifies the recovery point object that this cmdlet changes.

```yaml
Type: ASRRecoveryPoint
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReplicationProtectedItem
Specifies the Replication Protected Item object.

```yaml
Type: ASRReplicationProtectedItem
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DataEncryptionPrimaryCertFile
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

### -DataEncryptionSecondaryCertFile
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

### Microsoft.Azure.Commands.SiteRecovery.ASRJob

## NOTES

## RELATED LINKS

[Azure Site Recovery Cmdlets](./AzureRM.SiteRecovery.md)
