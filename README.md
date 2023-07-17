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


7) Install MySQL 5.5.62 (mysql-5.5.62-win32.msi)

![Screenshot (28)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/2c1ed243-ba80-4669-b295-2727cb678440)

Once installed, launch the configuration wizard for MySQL and select **_Standard Configuration_**. For the security settings, the username will always be root. Create a password and finish installation. 

![Screenshot (29)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/cc2583e4-2dd1-407e-a6b2-a0ad18ba3053)


8) Open IIS as an Admin. Once open, go to **_PHP Manager_** and click **_Register new PHP version_**. Browse to **_php-cgi_** in the PHP folder and click it for registation. Finally, restart web server


9) Install osTicket  v.1.15.8. Once installed, click on the file and move the upload file inside the osTicket folder to **_Windows:C_** -> **_inetpub_** -> **_wwwroot_**. Rename the upload folder to **_osTicket_**. Restart the web server in IIS.


10) In IIS, go to **_Sites_** -> **Default Web Sites_** -> **_osTicket_**. Click on **_Browse*.80_**. This will open the the osTicket Installer.

![Screenshot (31)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/e353890e-40bf-4380-a53d-a5d098b43a1f)


11) In IIS, go to **_Sites_** -> **Default Web Sites_** -> **_osTicket_**. Double click **_PHP Manager_** and click **_Enable or disable and extension_**. From here, enable **_php_imap.dll_**,**_php_intl.dll_**, and **_php.opcache.dll_*. Refresh the osTicket website for the changes to occur. 

![Screenshot (36)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/8f2b7d71-e809-4810-9bf1-3632998ba74c)


12) From the file explorer go to **_Windows:C_** -> **_inetpub_** -> **_wwwroot_** -> **_osTicket_** -> **_include_**. Rename the file **_ost-sampleconfig.php_** to **_ost-config.php_**. Go to **_ost-config.php_** properties and Disable inheritance -> Remove all. Then set New Permission -> Everyone -> All


13) Go back to osTicket installer and continue to fill out the following information (i.e. Helpdesk Name, Default email, etc)

![Screenshot (32)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/dbe6b44a-8a7f-445b-bc9c-346066d9b5e6)

14) Install HeidiSQL

![Screenshot (33)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/238da758-f334-4e93-94f7-4ef3f391f394)


15) Open HeidiSQL. Create a new session and connect to it

![Screenshot (37)](https://github.com/nickcaviness/osticket-prereqs/assets/137835904/66ae1422-e681-4785-a5f8-9e4ac3bbf57c)
















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
