Provision windows and linux VM resources with terraform on Azure

I will like to add the built in policies to scale the VMs automatically. We can do this by creating policies like this https://learn.microsoft.com/en-us/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-scale-in-policy

We will probably need to create a policy definition and assignment using terraform. Look into this https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/subscription_policy_assignment

Maybe also implement remediation so that policy takes effect at the resource level and not have to redeploy VM? 
