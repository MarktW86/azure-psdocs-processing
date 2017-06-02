---
title: Other ways to install Azure PowerShell | Microsoft Docs
description: How to install Azure PowerShell using the MSI package or the Web Platform Installer.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-resource-manager
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/docs-conceptual/other-install.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/docs-conceptual/other-install.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4eeb8dd94134977ba5c8e00ed61e2b1a029bef1d
open_to_public_contributors: true
---

# Other installation methods

Azure PowerShell has multiple installation methods. Using PowerShellGet with the PowerShell Gallery
is the preferred method. Azure PowerShell can be installed using the Web Platform Installer (WebPI)
or by using the MSI file available from
[GitHub](https://github.com/Azure/azure-powershell/releases/latest).

## Install using the Web Platform Installer

Installing the latest Azure PowerShell from WebPI is the same as it was for previous versions.
Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.

> [!NOTE]
> If you have previously installed Azure modules from the PowerShell Gallery, the installer
> automatically removes them. This simplifies your environment by ensuring that only one version
> of Azure PowerShell is installed. However, there are scenarios where you may need multiple
> versions installed at the same time.
>
> PowerShell Gallery modules install modules in
> `$env:ProgramFiles\WindowsPowerShell\Modules`. In contrast, the WebPI installer
> installs the Azure modules in `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.
>
> If an error occurs during install, you can manually remove the Azure* folders in your
> `$env:ProgramFiles\WindowsPowerShell\Modules` folder, and try the installation again.

Once the installation completes, your `$env:PSModulePath` setting should include the directories
containing the Azure PowerShell cmdlets. The following command can be used to verify that the Azure
PowerShell is installed properly.

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> There is a known issue that can occur when installing from WebPI. If your computer requires a
restart due to system updates or other installations, it may cause updates to `$env:PSModulePath` to
fail to include the path where Azure PowerShell is installed.

When attempting to load or execute cmdlets after installation, you can receive the following error
message:

```
PS C:\> Login-AzureRmAccount
Login-AzureRmAccount : The term 'Login-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Login-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Login-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

This error can be corrected by restarting the machine or importing the module using the fully
qualified path. For example:

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## Install using the MSI Package

Azure PowerShell can be installed using the MSI file available from
[GitHub](https://github.com/Azure/azure-powershell/releases/latest). If you have installed previous
versions of Azure modules, the installer automatically removes them. The MSI package installs
modules in `$env:ProgramFiles\WindowsPowerShell\Modules` but does not create version-specific
folders.