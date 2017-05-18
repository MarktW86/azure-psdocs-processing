---
title: Azure PowerShell Change Log | Microsoft Docs
description: This is a history of changes made to Azure PowerShell in the latest release.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-resource-manager
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload:
ms.date: 05/18/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/docs-conceptual/1.2.9/release-notes-azureps.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/docs-conceptual/1.2.9/release-notes-azureps.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/1886ae4675a95d2bdeb222cb28c9c5c7645fb848
open_to_public_contributors: true
---

# Release notes

This is a list of changes made to Azure PowerShell in this release.

## Version 1.2.9

Changes This Release

* AzureRm.AzureStackAdmin Module
    + Changes in the Add-AzureRmResourceProviderRegistration cmdlet for the support of Admin Azure
      resource manager and tenant azure resource manager split. A new parameter -ResourceManagerType
      has been added.
    + Removal of the parameters -AdminUri, -ApiVersion, -SubscriptionId and -Token from each
      cmdlets. We have been printing warnings that these parameters will be deprecated and now they
      got removed.
* AzureStackStorage module
    + Added new cmdlets to support container migration scenarios.
    + Removed cmdlets referring to internal components and underlying features.
* AzureRM.BootStrapper
    + Created new module to manage versions of Azure PowerShell cmdlets through the use of version
      profiles