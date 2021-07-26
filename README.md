# AzureAppServiceDomainAndDNS
JSON ARM template for deploying a domain you currently own into Azure as an App Service Domain and a DNS zone
## Introduction
To keep the integrity of your management, you can also request to transfer your domain name from a current registrar to Azure and manage it through Azure App Service Domains. This ARM template creates an Azure App Service Domain in addition to an empty DNS zone which could be used later for your DNS records.

## Instruction
You need to change follwoings in the JSON file based on your needs:

Parameters sescion
1. YourDomain.com: Your preferred domain name
2. YourIPaddress: Your computer valid IP address. You can find it by navigating to https://www.whatismyip.com
3. CurrentDateAndTime: in "yyyy-MM-ddTHH:mm:ss" format
4. YourAuthCode: The code used to authenticate for domain transfer

Variables sescion
1. YOURSUBSCRIPTIONNUMBER: Replace with your specific Azure subscription number
2. RESOURCEGROUPNAME: Replace with the resource group name you want to create the domain name zone in

After seting those parameters, you can use it to "Deploy a custom template" through Azure portal, which looks like following figure. 

![image](https://user-images.githubusercontent.com/54755447/126993302-1e07364a-ed99-46ac-a20f-b13357ef103d.png)
