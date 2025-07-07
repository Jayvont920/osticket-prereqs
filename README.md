<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Install/Enable Internet information Services (IIS) With CGI
- Download and unzip PHP files 
- Install C++ redistributable 
- Install MySQL and set username and password 
- Configure permissions and install osTicket

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/pgBLK3B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this first step, we are installing Internet Information Services with CGI (CGI is a dependency that osTicket needs for part of the web server) . To do so, we will navigate to the control panel in the start menu and click "Programs and Features". From there, we will click "Turn Windows features on or off" on the left side of the window and find IIS in the next window. To add CGI, we will expand "world Wide Web Services" then "Application Development Features" and click "CGI" then click "OK" to install.
</p>
<br />

<p>
<img src="https://i.imgur.com/UuFOkzP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now, we will to download the necessary PHP files, which are the files that osTicket needs to create tickets, manage users, and display the help desk interface in a web browser. Once we download the zip file from the PHP website, create a folder on the C:\ drive named "PHP" and extract the zip file to this location. 
</p>
<br />

<p>
<img src="https://i.imgur.com/suOmacW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, we want to download the latest C++ Redistributable. This is necessary due to the files within the PHP folder relying on the C++ runtime libraries in order to properly load.
</p>
<br />

<p>
<img src="https://imgur.com/yU58bei.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
