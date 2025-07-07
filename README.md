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

- Install/Enable Internet information Services (IIS) With CGI
- Download and unzip PHP files 
- Install C++ redistributable 
- Install MySQL and set username and password 
- Configure permissions and install osTicket

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/pgBLK3B.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
For the first step, we are installing Internet Information Services with CGI (CGI is a dependency that osTicket needs for part of the web server) . To do so, we will navigate to the control panel in the start menu and click "Programs and Features". From there, we will click "Turn Windows features on or off" on the left side of the window and find IIS in the next window. To add CGI, we will expand "world Wide Web Services" then "Application Development Features" and click "CGI" then click "OK" to install.
</p>
<br />

<p>
<img src="https://i.imgur.com/UuFOkzP.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now, we will to download the necessary PHP files, which are the files that osTicket needs to create tickets, manage users, and display the help desk interface in a web browser. Once we download the zip file from the PHP website, create a folder on the C:\ drive named "PHP" and extract the zip file to this location. 
</p>
<br />

<p>
<img src="https://i.imgur.com/suOmacW.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, we want to download the latest C++ Redistributable. This is necessary due to the files within the PHP folder relying on the C++ runtime libraries in order to properly load.
</p>
<br />

<p>
<img src="https://imgur.com/yU58bei.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this next step we will need to downnload and set up mySQL. The download can be found on mysql.com. This is necessary because osTicket relies on a database to retrieve, update, and manage support data efficiently. MySQL will be where osTicket will store or access the data needed to function properly. During setup, select "typical setup", then launch the configuration wizard after installation, lastly continue with "Standard Configuration" and create a username and password that is easy to remember.
</p>
<br />

<p>
<img src="https://imgur.com/TQogwJV.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open Internet Information Services (IIS) as an admin and register your PHP executable that we downloaded earlier within PHP Manager. After registering, reload IIS (open IIS, Stop and Start the server)
</p>
<br />

<p>
<img src="https://imgur.com/txbtN1X.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download the latest osTicket zip file and extract it to your desktop. Once extracted, copy the "upload" folder into "c:\inetpub\wwwroot" and rename "upload" to "osTicket". Make sure it is renamed exactly how it is seen here. Reload IIS like done in the previous step.
</p>
<br />

<p>
<img src="https://imgur.com/zzs9pTP.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within IIS, select sites the press the downward arrow on the left until you see the osTicket folder. Select osTicket then select "Browse *.80" which is seen on the left side of the screen. This will take us to the osTicket Installer website.
</p>
<br />

<p>
<img src="https://imgur.com/eeXyvr4.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we will rename "C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php" to "C:\inetpub\wwwroot\osTicket\include\ost-config.php". We are doing this because osTicket looks specifically for ost-config.php to load your site's configuration settings, such as database connection details. 
</p>
<br />

<p>
<img src="https://imgur.com/I09OOnz.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within the properties of ost-config.php, go to "Advanced" and select "Disable inheritance" in the botton left corner.
</p>
<br />

<p>
<img src="https://imgur.com/URCOCDj.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To add permissions, select "Add" in the bottom left corner then select "Select a principal". Next, type "Everyone" then check the box that says "Full Control". This will essentially give osTicket full control of the configuration file which is just being done for the sake of this instruction.
</p>
<br />

<p>
<img src="https://imgur.com/zzs9pTP.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, download and Run HeidiSQL.Select "New" in the bottom left corner and input the username and password that was set.(In this case, they are both "root"). HeidiSQL is being used to create a database within osTicket.
</p>
<br />

<p>
<img src="https://imgur.com/SrLh7Pz.png" height="1000%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside your browser, continue the install process for osTicket. In the "Database Settings" section, input the information that was used to set up a database within HeidiSQL. Once complete, select "Install Now" and you will have successfully installed and configured osTicket and installed all necessary files that it relies on. 
</p>
<br />
