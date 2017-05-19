---
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-7/Azure%20AD%20Cmdlets/docs-conceptual/PowerShell-logfile.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-7/Azure%20AD%20Cmdlets/docs-conceptual/PowerShell-logfile.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/79ba9960c15a8ef8b3259a44f308cc3d918ee65e
---
# Where can I find the PowerShell log file?

Azure AD PowerShell maintains a log file for diagnostic purposes. You can find this file here:

```powershell
C:\Users\<alias>\AppData\Local\Microsoft\AzureAD\Powershell\AzureADPowershell_<sessionStartTimeStamp>.log
```

The log file contains a time stamped record of all actions a cmdlet has executed. You can use this to analyze errors or just follow the execution path of a cmdlet or script.
