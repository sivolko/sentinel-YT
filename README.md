---
description: This is my first Cloud Native SIEM Project using MS Sentinel
---

# SIEM Project

## Objective :-&#x20;

To build a cloud native SIEM solution and monitor a Machine with process id 4624 (Success Log in )

### Architecture&#x20;

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

Steps :-

* Signup /Login for Azure&#x20;
* Create a RG - <[sentinelProject](https://portal.azure.com/#@hugs4bugs.me/resource/subscriptions/46ab4919-3d35-463c-a2cd-7896727d7653/resourceGroups/sentinelProject)>
* To install AMA (Azure Monitoring Agent) we need a Machine so we're deploying Win 10 client VM inside Azure&#x20;
* Create a VM <[sentinelVM](https://portal.azure.com/#@hugs4bugs.me/resource/subscriptions/46ab4919-3d35-463c-a2cd-7896727d7653/resourceGroups/sentinelProject/providers/Microsoft.Compute/virtualMachines/sentinelVM)>- OS - Win 10 - Bastion to connect&#x20;
* Create Log Analytics workspace&#x20;
* Deploy MS Sentinel inside same Log Analytics workspace&#x20;
* Install AMA from Content Hub -- Windows Security Events

