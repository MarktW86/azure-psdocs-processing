---
title: Manage Azure subscriptions with Azure PowerShell | Microsoft Docs
description: Manage Azure subscriptions with Azure PowerShell
keywords: Azure PowerShell, subscription
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-resource-manager
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/docs-conceptual/manage-subscriptions-azureps.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/docs-conceptual/manage-subscriptions-azureps.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/379641e1d19b18dec54244dce5910aa3f4d6d991
open_to_public_contributors: true
---

# Manage multiple Azure subscriptions

If you are brand new to Azure, you probably only have a single subscription. But if you have been
using Azure for a while, you may have created multiple Azure subscriptions. You can configure Azure
PowerShell to execute commands against a particular subscription.

1. Get a list of all subscriptions in your account.

    ```powershell
    Get-AzureRmSubscription
    ```

    ```
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Production Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My DevTest Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

2. Set the default.

    ```powershell
    Select-AzureRmSubscription -SubscriptionName "My Demos"
    ```

3. Verify the change by running the `Get-AzureRmContext` cmdlet.

    ```powershell
    Get-AzureRmContext
    ```

    ```
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

Once you set your default subscription, all subsequent Azure PowerShell commands run against this
subscription.
