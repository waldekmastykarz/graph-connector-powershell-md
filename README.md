#

## Prerequisites

- [Microsoft Graph PowerShell SDK](https://learn.microsoft.com/powershell/microsoftgraph/installation?view=graph-powershell-1.0)
- [Microsoft.PowerShell.SecretManagement](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.secretmanagement/?view=ps-modules)
- [Microsoft.PowerShell.SecretStore](https://learn.microsoft.com/powershell/module/microsoft.powershell.secretstore/?view=ps-modules)
- [powershell-yaml](https://www.powershellgallery.com/packages/powershell-yaml/0.4.7)

## MPA

```powershell
# Ensure you've got a default secret store configured, by running
Get-SecretVault
# If nothing shows up, run
Register-SecretVault -Name LocalStore -ModuleName Microsoft.PowerShell.SecretStore -DefaultVault
# Create Entra app
./Initialize-EntraApp.ps1
# Create external connection
./Initialize-EntraExternalConnection.ps1
# Import content
./Import-Content.ps1
```
