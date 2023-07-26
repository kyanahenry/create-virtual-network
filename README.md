
<p align="center">
<img srcset="https://connectoricons-prod.azureedge.net/u/shgogna/globalperconnector-train1/1.0.1639.3312/azurevm/icon.png" src="https://connectoricons-prod.azureedge.net/u/shgogna/globalperconnector-train1/1.0.1639.3312/azurevm/icon.png" alt="Azure VM" class="">"
</p>

<h1>Create a Virtual Machine and Deploy a Web Server</h1>
This tutorial outlines how to set up an Ubuntu Virtual Machine and install a Nextcloud server, then launch it via a public IP address.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Bastion
- Ubuntu
- NextCloud

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Project Outline</h2>

- Create a Virtual Network, then Protect a Subnet using a NSG
- Create a Virtual Machine, Deploy via Bastion
- Publish an IP address, then create a DNS label

<p>
<img src="https://github.com/kyanahenry/create-virtual-network/assets/137842747/8d581ed4-c2ce-4b87-9f99-4335acd5631c">
</p>
<p>
First, I created a Resource Group in Microsoft Azure then set up a Virtual Network inside the Resource Group. As shown above, I've created a Network Security Group and added it to our subnet to help filter inbound and outbound traffic between the internet and Azure resources. 
</p>
<br />

<p>
<img src="https://github.com/kyanahenry/create-virtual-network/assets/137842747/81eebcdb-97eb-4714-81dd-9d75644ce921"/>
</p>
<p>
Next, I created a Virtual Machine in Azure utilizing Ubuntu servers. I connected to the Virtual Machine using SSH via Bastion (as shown above). 
</p>
<br />

<p>
<img src="https://github.com/kyanahenry/create-virtual-network/assets/137842747/b0311768-4b62-4aca-beb7-d1fa5fffd67e"/>
</p>
<p>
After deploying Bastion, I installed Nextcloud on our Virtual Machine and associated a public IP to the server. Lastly, I set up a DNS entry for the public IP address in order to access it. 
</p>
