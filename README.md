<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>List of Prerequisites</h2>

- Azure tenant needs to be created.
- Need to have an active Microsoft Azure subscription.
- Need to create a Resource Group within Microsoft Azure.
- Need to create a Virtual Machine within your Microsoft Azure Resource Group.
- Need to create a subnet.

<h2>Installation Steps</h2>

<p>
<img width="1242" alt="image" src="https://github.com/CarlosVanzego/osticket-prereqs/assets/129208650/4aa9c2ec-1fd6-4ce3-ae78-1615a0d7c0db">
</p>
<p>
Log in to the Azure portal (portal.azure.com) using your Azure account credentials.
In the Azure portal, click on "Virtual Machines" from the left-hand menu and then select "Create."
Choose the desired configuration for your VM, including the region, size, and operating system. Select a Windows-based OS that is compatible with osTicket, such as Windows Server 2016 or Windows Server 2019.
Configure the other settings, such as the username and password for the VM, and click on "Create" to provision the VM..
</p>
<br />

<p>
<img width="1437" alt="image" src="https://github.com/CarlosVanzego/osticket-prereqs/assets/129208650/70c4180c-1271-40ac-a922-be78a601be07">
</p>
<p>
Once the VM is created, navigate to the "Virtual Machines" section in the Azure portal and select your newly created VM.
Copy the "Public IP Address". Open up the "Microsoft Remote Desktop" App, click "Add PC" then paste the IP Address in the "PC Name" field and click add" which allows you to connect to the VM. Open the VM file and enter the username and password you specified during the VM creation process to establish a remote desktop connection to the VM.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once connected to the VM, open a web browser and download the latest version of osTicket from the official website (osticket.com).
Transfer the downloaded osTicket files to the VM by either using a file transfer protocol (FTP) client or directly through the RDP session by copying and pasting the files.
Extract the osTicket files in a desired location on the VM, such as the default web server root folder (e.g., "C:\inetpub\wwwroot\osticket").
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open a web browser within the RDP session and enter the IP address or hostname of the VM to access osTicket.
The osTicket installation wizard should automatically start. Follow the on-screen instructions to set up the initial configuration, including database connection details, administrator account creation, and other settings.
Once the installation is complete, you should be able to access the osTicket help desk system by entering the VM's IP address or hostname in a web browser from any device on your network.
</p>
<br />
