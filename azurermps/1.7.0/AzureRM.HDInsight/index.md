---
Module Name: AzureRM.HDInsight
Module Guid: XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
Locale: en-US
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v1.1.4/AzureRM.HDInsight.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v1.1.4/AzureRM.HDInsight.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: conceptual
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: hdinsight
Add-AzureRmHDInsightClusterIdentity: HD Insights
Add-AzureRmHDInsightConfigValues: HD Insights
Add-AzureRmHDInsightMetastore: HD Insights
Add-AzureRmHDInsightScriptAction: HD Insights
Add-AzureRmHDInsightStorage: HD Insights
Get-AzureRmHDInsightCluster: HD Insights
Get-AzureRmHDInsightJob: HD Insights
Get-AzureRmHDInsightJobOutput: HD Insights
Get-AzureRmHDInsightPersistedScriptAction: HD Insights
Get-AzureRmHDInsightProperties: HD Insights
Get-AzureRmHDInsightScriptActionHistory: HD Insights
Grant-AzureRmHDInsightHttpServicesAccess: HD Insights
Grant-AzureRmHDInsightRdpServicesAccess: HD Insights
Invoke-AzureRmHDInsightHiveJob: HD Insights
New-AzureHDInsightClusterIdentity: Others
New-AzureRmHDInsightCluster: HD Insights
New-AzureRmHDInsightClusterConfig: HD Insights
New-AzureRmHDInsightHiveJobDefinition: HD Insights
New-AzureRmHDInsightMapReduceJobDefinition: HD Insights
New-AzureRmHDInsightPigJobDefinition: HD Insights
New-AzureRmHDInsightSqoopJobDefinition: HD Insights
New-AzureRmHDInsightStreamingMapReduceJobDefinition: HD Insights
Remove-AzureRmHDInsightCluster: HD Insights
Remove-AzureRmHDInsightPersistedScriptAction: HD Insights
Revoke-AzureRmHDInsightHttpServicesAccess: HD Insights
Revoke-AzureRmHDInsightRdpServicesAccess: HD Insights
Set-AzureRmHDInsightClusterSize: HD Insights
Set-AzureRmHDInsightDefaultStorage: HD Insights
Set-AzureRmHDInsightPersistedScriptAction: HD Insights
Start-AzureRmHDInsightJob: HD Insights
Stop-AzureRmHDInsightJob: HD Insights
Submit-AzureRmHDInsightScriptAction: HD Insights
Use-AzureRmHDInsightCluster: HD Insights
Wait-AzureRmHDInsightJob: HD Insights
_isModulePage: true
---

# AzureRM.HDInsight Module
## Description
The topics in this section document the Azure PowerShell cmdlets for Microsoft Azure HDInsight in the Azure Resource Manager (ARM) framework. These cmdlets are used to manage HDInsight clusters and the jobs that run on them. The cmdlets exist in the Microsoft.Azure.Commands.HDInsight namespace.

## AzureRM.HDInsight Cmdlets
### [Add-AzureRmHDInsightConfigValues](Add-AzureRmHDInsightConfigValues.md)
Adds a Hadoop configuration value customization and/or a Hive shared library customization to a cluster configuration object.

### [Add-AzureRmHDInsightMetastore](Add-AzureRmHDInsightMetastore.md)
Adds a SQL Database to serve as a Hive or Oozie metastore to a cluster configuration object.

### [Add-AzureRmHDInsightScriptAction](Add-AzureRmHDInsightScriptAction.md)
Adds a script action to a cluster configuration object.

### [Add-AzureRmHDInsightStorage](Add-AzureRmHDInsightStorage.md)
Adds an Azure Storage key to a cluster configuration object.

### [Get-AzureRmHDInsightCluster](Get-AzureRmHDInsightCluster.md)
Gets and lists all of the Azure HDInsight clusters associated with the current subscription or a specified resource group, or retrieves a specific cluster.

### [Get-AzureRmHDInsightJob](Get-AzureRmHDInsightJob.md)
Gets the list of jobs from a cluster and lists them in reverse chronological order, or retrieves a specific job.

### [Get-AzureRmHDInsightJobOutput](Get-AzureRmHDInsightJobOutput.md)
Gets the log output for a job from the storage account associated with a specified cluster.

### [Get-AzureRmHDInsightProperties](Get-AzureRmHDInsightProperties.md)
Gets properties about the HDInsight service, such as available locations and capacity.

### [Grant-AzureRmHDInsightHttpServicesAccess](Grant-AzureRmHDInsightHttpServicesAccess.md)
Grants HTTP access to the cluster.

### [Grant-AzureRmHDInsightRdpServicesAccess](Grant-AzureRmHDInsightRdpServicesAccess.md)
Grants RDP access to the Windows cluster.

### [Invoke-AzureRmHDInsightHiveJob](Invoke-AzureRmHDInsightHiveJob.md)
Submits a Hive query to an HDInsight cluster and retrieves query results in one operation.

### [New-AzureHDInsightClusterIdentity](New-AzureHDInsightClusterIdentity.md)
{{Fill in the Synopsis}}

### [New-AzureRmHDInsightCluster](New-AzureRmHDInsightCluster.md)
Creates an Azure HDInsight cluster in the specified resource group for the current subscription.

### [New-AzureRmHDInsightClusterConfig](New-AzureRmHDInsightClusterConfig.md)
Creates a non-persisted cluster configuration object that describes an Azure HDInsight cluster configuration.

### [New-AzureRmHDInsightHiveJobDefinition](New-AzureRmHDInsightHiveJobDefinition.md)
Creates a Hive job object.

### [New-AzureRmHDInsightMapReduceJobDefinition](New-AzureRmHDInsightMapReduceJobDefinition.md)
Creates a MapReduce job object.

### [New-AzureRmHDInsightPigJobDefinition](New-AzureRmHDInsightPigJobDefinition.md)
Creates a Pig job object.

### [New-AzureRmHDInsightSqoopJobDefinition](New-AzureRmHDInsightSqoopJobDefinition.md)
Creates a Sqoop job object.

### [New-AzureRmHDInsightStreamingMapReduceJobDefinition](New-AzureRmHDInsightStreamingMapReduceJobDefinition.md)
Creates a Streaming MapReduce job object.

### [Remove-AzureRmHDInsightCluster](Remove-AzureRmHDInsightCluster.md)
Removes the specified HDInsight cluster from the current subscription.

### [Revoke-AzureRmHDInsightHttpServicesAccess](Revoke-AzureRmHDInsightHttpServicesAccess.md)
Disables HTTP access to the cluster.

### [Revoke-AzureRmHDInsightRdpServicesAccess](Revoke-AzureRmHDInsightRdpServicesAccess.md)
Disables RDP access to a Windows cluster.

### [Set-AzureRmHDInsightClusterSize](Set-AzureRmHDInsightClusterSize.md)
Sets the number of Worker nodes in a specified cluster.

### [Set-AzureRmHDInsightDefaultStorage](Set-AzureRmHDInsightDefaultStorage.md)
Sets the default Storage account setting in a cluster configuration object.

### [Start-AzureRmHDInsightJob](Start-AzureRmHDInsightJob.md)
Starts a defined Azure HDInsight job on a specified cluster.

### [Stop-AzureRmHDInsightJob](Stop-AzureRmHDInsightJob.md)
Stops a specified running job on a cluster.

### [Use-AzureRmHDInsightCluster](Use-AzureRmHDInsightCluster.md)
Selects a cluster to be used with the Invoke-RmAzureHDInsightHiveJob cmdlet.

### [Wait-AzureRmHDInsightJob](Wait-AzureRmHDInsightJob.md)
Waits for the completion or failure of a specified job.

