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

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Creating a virtual machine in Microsoft Azure and remote desktop to it
- Open a file with the necessary programs that will be used to create the OS ticketing system

<h2>Installation Steps</h2>

1) First, connect to the virtual machine and install Internet Information Service or IIS. To do this, go to **_Control Panel_**. From there, click on **_Programs_** and then click on **_Turn Windows features on or off_**. Next, expand the following tab **_Internet Information Service_** which will lead to **_Application Development Features_**. Enable **_CGI_**. Once enabled, go to **_Common HTTP Features_** and enable everything underneath the tab. 

![Screenshot (21)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/b32b2f8e-5237-45e5-aab5-a7325a6ef6ee)

Type the IP Address **_127.0.0.1_** in a website search bar. Doing so will show the default IIS page. 

![Screenshot (22)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/79029a8f-c634-46ff-8485-3b8d48f34eb2)


2) Install PHP Manager (PHPManagerForllS_V1.5.0.msi)

![Screenshot (23)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/4ac208d9-5e24-4f6c-a1a0-e7c33b197cf3)


3) Install the Rewrite Module (rewrite_amd64_en-US.msi)

 ![Screenshot (24)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/7d7ca116-fc3e-41e4-8a91-dc6eed003263)


4) Create the directory **_C:\PHP_** on the Windows C Drive

![Screenshot (25)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/7f0c4b05-ce0d-4d6c-b8ab-daa779164c2d)


5) Install PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip). Once installed, unzip the program into **_C:\PHP_**

![Screenshot (25)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/e9c747f2-ddb2-48c6-a87b-7063e98c22b0)


6) Install Microsoft Visual C++ Redistributable program (VC.redist.x86.exe)

![Screenshot (27)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/794804d3-6f38-4b5d-aa3e-cee0d05474d5)



















</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
