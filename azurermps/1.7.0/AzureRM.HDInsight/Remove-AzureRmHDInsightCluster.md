---
external help file: Microsoft.Azure.Commands.HDInsight.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/02/2017 17:05 PM
ms.date: 05/02/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v1.1.4/Remove-AzureRmHDInsightCluster.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v1.1.4/Remove-AzureRmHDInsightCluster.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/fdff926f5dd35f9020f210f87b450464ba162edc
ms.topic: reference
ms.service: hdinsight
---

# Remove-AzureRmHDInsightCluster

## SYNOPSIS
Removes the specified HDInsight cluster from the current subscription.

## SYNTAX

```
Remove-AzureRmHDInsightCluster [-ClusterName] <String> [-ResourceGroupName <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The Remove-AzureRmHDInsightCluster cmdlet removes the specified HDInsight service cluster from a subscription.
This operation also deletes any data stored in the Hadoop Distributed File System (HDFS) on the cluster.
Data stored in the associated Azure Storage account is not deleted.
Data stored in external metastores is not deleted.

## EXAMPLES

### --------------------------  Example 1: Delete an Azure HDInsight cluster.  --------------------------
@{paragraph=PS C:\\\>}



```
PS C:\&gt;Remove-AzureRmHDInsightCluster -ClusterName "your-hadoop-001"
```

## PARAMETERS

### -ClusterName
Specifies the name of the cluster.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
@{Text=}

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
@{Text=}

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
Specifies the name of the resource group.

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
Keywords: azure, azurerm, arm, resource, management, manager, hadoop, hdinsight, hd, insight

## RELATED LINKS

