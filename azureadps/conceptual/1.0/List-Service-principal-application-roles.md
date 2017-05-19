---
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-7/Azure%20AD%20Cmdlets/docs-conceptual/List-Service-principal-application-roles.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/RobdeJong-patch-7/Azure%20AD%20Cmdlets/docs-conceptual/List-Service-principal-application-roles.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/f4f8f8e62d49d3b391f0437294292a7914a5c8c3
---
# List all application role assignments for all service principals in your directory

If you want to list all service principals that have access to applications in your directory you can use the below script. The script will get all service principals in your directory, then for each service principal retrieve the service principal's application role assignments and will list the application roles that are assigned to the service principal.
```powershell
# Get all service principals, and for each one, get all the app role assignments, 
# resolving the app role ID to it's display name. 
Get-AzureADServicePrincipal | % {

  # Build a hash table of the service principal's app roles. The 0-Guid is
  # used in an app role assignment to indicate that the principal is assigned
  # to the default app role (or rather, no app role).
  $appRoles = @{ "$([Guid]::Empty.ToString())" = "(default)" }
  $_.AppRoles | % { $appRoles[$_.Id] = $_.DisplayName }

  # Get the app role assignments for this app, and add a field for the app role name
  Get-AzureADServiceAppRoleAssignment -ObjectId ($_.ObjectId) | % {
    $_ | Add-Member "AppRoleDisplayName" $appRoles[$_.Id] -Passthru
  }
}
```