# General notes on Azure

Using PowerShell and Azure Module

1. Install Azure Module for PowerShell

2. Connect to your Azure account. Note that the TenantId will come in if you use MFA in your Azure subscription. If you attempt to connect to Azure without specifying TenantID and if MFA is enabled, the error message will tell you the exact TenantID to use. 

```PowerShell

Connect-AzAccount -TenantId 45794f26-9e1d-4849-aa49-601317b98dc1

```

To find the TenantID from the webUI, go to Azure Active Directory > Overview

![tenantID](https://xxxx)

3. Switching between Azure subscriptions if you have multiple ones
