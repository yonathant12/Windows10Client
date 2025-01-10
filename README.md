<h1>Setting up Windows 10 Client</h1>

<h2>Overview</h2>
Setting up a Windows 10 client on VMware Workstation 17 Pro involves creating a new virtual machine, configuring hardware settings, installing Windows 10 from an ISO file, and installing VMware Tools for enhanced functionality. Once the Windows 10 client is set up, I will verify that its IP address is within the defined scope and ping the Windows Server to ensure connectivity between the two machines.
<br />


<h2>Operating System and Software Used</h2>

- <b>VMware Workstation 17 Pro</b>
- <b>Windows 10 Pro</b> 

<h2>Lab walk-through:</h2>

<p align="center">
Click the "File" option on the top left and select "New Virtual Machine". Choose the Custom option and hit next.<br/>
<img src="https://i.imgur.com/L7q5mZ5.png" height="60%" width="60%"/>
<br />
<br />
Select the "I will install the operating system later" option and click next.<br/>
<img src="https://i.imgur.com/nEopp5i.png" height="60%" width="60%"/>
<br />
<br />
Select Microsoft Windows as the Guest operating system and choose Windows 10 x64 as the Version, then click next.<br/>
<img src="https://i.imgur.com/Ade2pz5.png" height="60%" width="60%"/>
<br />
<br />
Press next on the "Name the Virtucal Machine" screen. Select BIOS as Firmware Type and click next.<br/>
<img src="https://i.imgur.com/fhKOpZM.png" height="60%" width="60%"/>
<br />
<br />
Leave the "Processor Configuration" screen as default. Increase "Memory for the Virtual Machine" from 2GB to 4GB.<br/>
<img src="https://i.imgur.com/8sk9Rz1.png" height="60%" width="60%"/>
<br />
<br />
Choose "Use host-only networking" as the Network Type and click next.<br/>
<img src="https://i.imgur.com/zbfRFgu.png" height="60%" width="60%"/>
<br />
<br />
Choose "LSI Logic SAS (Recommended)" as the I/O Controller Type and click next.<br/>
Choose "NVMe (Recommended)" as the Disk Type and click next.<br/>
Choose "Create a new virtual disk" on the Select a Disk screen and click next.<br/>
Leave "Disk Capacity" as the recommended amount which is 60GB, select "Split virtual disk into multiple files", and then click next.<br/>
Leave "Disk File" as default and click next.<br/>
Verify the following setting and click finish.<br/>
<img src="https://i.imgur.com/2Wv2G3f.png" height="60%" width="60%"/>
<br />
<br />
Click "Edit virtual machine settings.<br/>
<img src="https://i.imgur.com/90vIvfl.png" height="60%" width="60%"/>
<br />
<br />
Select CD/DVD (SATA), choose the "Use ISO image file:" and click browse. Find the Windows 10 x64 ISO and click ok.<br/>
<img src="https://i.imgur.com/lHNYyCi.png" height="60%" width="60%"/>
<br />
<br />
Click "Power on this virtual machine"<br/>
<img src="https://i.imgur.com/V7A1oMr.png" height="60%" width="60%"/>
<br />
<br />
Once the Windows Setup comes on, click next and then click the Install now button.<br/>
<img src="https://i.imgur.com/GStu1pS.png" height="60%" width="60%"/>
<br />
<br />
Click the "I don't have a product key" button on Activate Windows screen.<br/>
<img src="https://i.imgur.com/pmeJ2Fs.png" height="60%" width="60%"/>
<br />
<br />
Select Windows 10 Pro as the operating system and click next.<br/>
<img src="https://i.imgur.com/omuGfm9.png" height="60%" width="60%"/>
<br />
<br />
Accept the license terms and click next.<br/>
Select Custom for the intallation type.<br/>
<img src="https://i.imgur.com/WaqQ5bb.png" height="60%" width="60%"/>
<br />
<br />
Click next on the "Where do you want to install Windows" screen.<br/>
Wait for Windows to install.<br/>
<img src="https://i.imgur.com/64s8CIb.png" height="60%" width="60%"/>
<br />
<br />
Once the Windows installation is finished. Select your region and click yes.<br/>
Select your keyboard layout and click yes.<br/>
Click skip when asked to add a second keyboard layout.<br/>
Select "Set up for personal use" and click next.<br/>
<img src="https://i.imgur.com/hxwMCEP.png" height="60%" width="60%"/>
<br />
<br />
On the "Let's add your account" screen, click Offline account at the bottom left.<br/>
Select Limited experience at the bottom left.<br/>
Setup a name, a password, and security questions.<br/>
<img src="https://i.imgur.com/sbrRFJS.png" height="60%" width="60%"/>
<br />
<br />
On the "Always have access to your recent browsing data" screen, click not now.<br/>
Turn all privacy settings to "No" and click accept.<br/>
On the "Let's customize your experience" screen, click skip.<br/>
On the "Let Cortana help you get things done" select not now.<br/>
Once that it finished, click the VM button at the top left, and then select "Install VMware Tools".<br/>
<img src="https://i.imgur.com/MxCbAYF.png" height="60%" width="60%"/>
<br />
<br />
Open up File Explorer and double click on "DVD Drive (D:) VMware Tools".<br/>
<img src="https://i.imgur.com/KejSXVz.png" height="60%" width="60%"/>
<br />
<br />
Click next on the "Welcome to the installation wizard for VMware Tools" screen.<br/>
<img src="https://i.imgur.com/10Dvy2t.png" height="60%" width="60%"/>
<br />
<br />
Select Typical as the setup type and click next.<br/>
Click install on the "Ready to intall VMware Tools" screen.<br/>
Click finish once it's completed.<br/>
Click Yes when asked to restart.<br/>
<img src="https://i.imgur.com/qp5Qslw.png" height="60%" width="60%"/>
<br />
<br />
Once the machine has restarted, log back in and open up Command Prompt.<br/>
Type in "ipconfig /all" to verify the IP address, the DHCP server and default gateway.<br/>
<img src="https://i.imgur.com/lFJJcnk.png" height="60%" width="60%"/>
<br />
<br />
Ping both Google and our domain server to verify internet connectivity, DNS resolution, and network infrastructure.<br/>
<img src="https://i.imgur.com/6EA48JC.png" height="60%" width="60%"/>
<br />
<br />
Open Windows Settings and select System.<br/>
Select About then scroll down and click "Rename this Pc (advanced)".<br/>
<img src="https://i.imgur.com/bhvbJrc.png" height="60%" width="60%"/>
<br />
<br />
Select change.<br/>
<img src="https://i.imgur.com/ZMHaf5L.png" height="60%" width="60%"/>
<br />
<br />
Enter a computer name then select Domain and enter the domain name to add this machine to the domain.<br/>
<img src="https://i.imgur.com/x8Td4Go.png" height="60%" width="60%"/>
<br />
<br />
Login with one of the users we created.<br/>
<img src="https://i.imgur.com/CqalDIv.png" height="60%" width="60%"/>
<br />
<br />
Click ok both of the "Chnange Name/Domain Changes" pop-ups. Then select restart now<br/>
Login with one of the users we created.<br/>
<img src="https://i.imgur.com/yB72BHm.png" height="60%" width="60%"/>
<br />
<br />
Open up Command Prompt.<br/>
Enter "whoami" to verify the current user.<br/>
<img src="https://i.imgur.com/tLdlU0t.png" height="60%" width="60%"/>
<br />
<br />
Log back in to the Windows Server 2019.<br/>
On Server Manager, click Tools, and then select "Active Directory Users and Computer".<br/>
Select the Computers folder to verify that the Windows 10 machine has been added to the domain.<br/>
<img src="https://i.imgur.com/aZQmD63.png" height="60%" width="60%"/>
<br />
<br />
On Server Manager, click Tools, and then select "DHCP".<br/>
Expand the Scope folder then select the Address Leases folder to see the IP address given to the Windows 10 machine.<br/>
<img src="https://i.imgur.com/bPYxu3s.png" height="60%" width="60%"/>
<br />
<br />
</p>
