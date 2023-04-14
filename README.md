# Azure Vwan with S2S

This creates a vwan and a couple of spoke vnets with VM's connected to the vhub but adds an onprem vnet with a S2S tunnel to the vhub. You'll be prompted for the resource group name, location where you want the resources created, your public ip and username and password to use for the VM's. NSG's are placed on the default subnets of each vnet allowing RDP access from your public ip.

The topology will look like this:

![wvanlabwithS2S](https://user-images.githubusercontent.com/128983862/231878058-c3e1b080-727d-401a-baf6-f2a14cae40ca.png)

You can run Terraform right from the Azure cloud shell by cloning this git repository with "git clone https://github.com/quiveringbacon/AzureVwanwithS2S.git ./terraform".

Then, "cd terraform" then, "terraform init" and finally "terraform apply -auto-approve" to deploy.
