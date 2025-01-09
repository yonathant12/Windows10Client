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
<img src="https://i.imgur.com/nEopp5i.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
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











</p>
