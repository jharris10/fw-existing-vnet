# Azure-Firewall-into-existing-environment

[<img src="http://azuredeploy.net/deploybutton.png"/>](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fjharris10%2Ffw-existing-vnet%2Fmaster%2FAdd-New-Firewall-AzureDeploy.json)

This template was created to support the deployment of a 3 interface Palo Alto Networks firewall into an existing Microsoft Azure environment that has the following items already deployed:

                    -Load Balancer - If being used
                    -Availability Set for the Firewall
                    -VNET - with subnets
                    -Resource Group for Firewall
            

FEATURES:
- The firewall deploys with 3 interfaces.  1 MGMT and 2 data plane into an existing environment.
- It is possible to choose the version of software the firewall is running. 7.1 or 8.0 (Latest)
- The deployment SKU can also be choosen during deployment.  BYOL, Bundle1 or Bundle2 are the available options.
- Static IP addresses assignment is used for all the firewall interfaces.


The following Storage Account types are supported:

                    -Premium_LRS
                    
The following VMs are supported:

                    -Standard_D3
                    -Standard_D4
                    -Standard_D3_v2
                    -Standard_D4_v2
                    -Standard_DS3_v2
                    -Standard_DS4_v2
        
NOTE: Make sure the VMs are supported in the specific Storage Account Type and Azure Region.

After deploying, this firewall can be intetgrated into a load balancer setup via the Azure Portal.

