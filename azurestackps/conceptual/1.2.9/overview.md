---
title: Overview of the Azure Stack PowerShell | Microsoft Docs
description: Overview of Azure Stack PowerShell installation and configuration.
author: SnehaGunda
manager: Byronr
ms.product: azure-stack
ms.service: powershell
ms.devlang: powershell
ms.topic: reference
ms.author: sngun
ms.manager: byronr
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/docs-conceptual/overview.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/AzureStack/docs-conceptual/overview.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/8ae5d5454305d13e321c3e578e76e8dbf4321453
open_to_public_contributors: true
---

# Azure Stack PowerShell 

Azure Stack requires the following two PowerShell modules:  

1. The Azure Stack compatible **AzureRM** module which is available by installing the **2017-03-09-profile** API Version Profile. The cmdlets installed by using this profile can be used by the Azure Stack cloud administrators and the tenants. To learn about the PowerShell cmdlets available in this profile, see the [reference](/azure/overview?view=azurermps-1.2.9) section.  

2. The **1.2.9** version of the **AzureStack** module. The cmdlets installed by using this module can be used by Azure Stack cloud administrators only. Administrator can perform operations such as manage offers, plans, services, quotas, etc. by using the PowerShell cmdlets provided by this module. To learn about the PowerShell cmdlets available in this module, see the reference section.

## Next Steps

* [Install PowerShell for Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install)
* [Configure PowerShell for use with Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-configure)


