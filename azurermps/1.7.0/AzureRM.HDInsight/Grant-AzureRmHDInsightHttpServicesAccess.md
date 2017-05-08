---
external help file: Microsoft.Azure.Commands.HDInsight.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/02/2017 17:05 PM
ms.date: 05/02/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/DuncanmaMSFT-patch-1/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v1.1.4/Grant-AzureRmHDInsightHttpServicesAccess.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/DuncanmaMSFT-patch-1/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v1.1.4/Grant-AzureRmHDInsightHttpServicesAccess.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/fdff926f5dd35f9020f210f87b450464ba162edc
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: hdinsight
---

# Grant-AzureRmHDInsightHttpServicesAccess

## SYNOPSIS
Grants HTTP access to the cluster.

## SYNTAX

```
Grant-AzureRmHDInsightHttpServicesAccess [-ClusterName] <String> [-HttpCredential] <PSCredential>
 [-ResourceGroupName <String>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The Grant-AzureRmHDInsightHttpServicesAccess cmdlet grants HTTP access to an Azure HDInsight cluster using ODBC, Ambari, Oozie and web services.

## EXAMPLES

### --------------------------  Example 1: Grant HTTP access to an Azure HDInsight cluster  --------------------------
@{paragraph=PS C:\\\>}



```
PS C:\&gt; # Cluster info
        $clusterName = "your-hadoop-001"
        $clusterCreds = Get-Credential

        Grant-AzureRmHDInsightHttpServicesAccess 
            -ClusterName $clusterName `
            -HttpCredential $newClusterCreds
```

This command grants HTTP access to the cluster named 'your-hadoop-001'.

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

### -HttpCredential
Specifies the cluster login (HTTP) credentials for the cluster.

```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
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

[Revoke-AzureRmHDInsightHttpServicesAccess]()

