# Office 365 DNS Deployment

## Description

Will deploy most of the needed DNS Records you need for a Domain to be set up with Office 365.

# Required Parameters

#### dnsZone

Name of the dnsZone to deploy with DNS Records, for an Office 365. If used against and existing DNS Zone in Azure, it will add the Record.

## Example on Deployments from PowerShell using this Template

```powershell
$TemplateURL = "https://raw.githubusercontent.com/dotStryhn/ARMDeployments/master/Office365.DNS.Deployment/Office365.DNS.Deployment.json"
New-AzResourceGroupDeployment -ResourceGroupName YourResourceGroup -TemplateUri $TemplateURL -dnsZone yourdomain.com
```