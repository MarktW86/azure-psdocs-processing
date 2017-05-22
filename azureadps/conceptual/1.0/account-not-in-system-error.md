---
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/VinceSmith-patch-1/Azure%20AD%20Cmdlets/docs-conceptual/account-not-in-system-error.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/VinceSmith-patch-1/Azure%20AD%20Cmdlets/docs-conceptual/account-not-in-system-error.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/81e81b86d71386b0190efc026547939508cf3387
---
# I get an error "\[your account] isn't in our system"

You can see this error message if the Connect-AzureAD cmdlet fails. There are several possible causes:

1. You actually typed in an account name that doesn't exist because there is a typo in the name. 
 Remedy: retype the account name, this time don't make the typing error :) 
2. The account exists but is in a different Azure Environment
Example: You're working in the German cloud but you didn't specify the German cloud as the target in your Connect-AzureAD cmdlet call.
 Remedy: Specify the AzureEnvironmentName in the Connect-AzureAd cmdlet call, like this:

```powershell
Connect-AzureAD -AzureEnvironmentName AzureGermanyCloud
```

You can specify the following values for -AzureEnvironmentName:

+ AzureCloud
+ AzureChinaCloud
+ AzureUSGovernment
+ AzureGermanyCloud
 
