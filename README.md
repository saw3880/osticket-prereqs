# osticket-prereqs<p align="center">
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

- have A azure tenat
- A already created azure subscription
- have a resource group within your subscription
- made a azure VM

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/is4bn70.png " height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once your prerequisites have been met your going to copy and paste your vm ip address and log in using the info that was used to create your vm.
  next you will install iis or internet imformation services to run osticket, in windows start menu you will go to control panel then                               under programs there will be windows features turn on iis and also cgi which is needed to to run php manager which osticket runs off of. 
  
</p>
<br />

<p>
<img src="https://i.imgur.com/05H2T1n.png " height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Another program that is needed to run os ticket is rewrite module once downloaded, you will need to make a folder for php manager to download php too
 then another needed program is  VC_redist.x86.exe all should be going into the php folder next program is (mysql-5.5.62-win32.msi) once downloaded
  you must make a name and password for mysql
</p>
<br />

<p>
<img src="https://i.imgur.com/hHmcR9a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once all required programs have been installed you must do some configuration, from start menu enter iis run as administrator then Register PHP from within IIS
restart iis.finally download osticket extract and copy to a special folder  name  c:\inetpub\wwwroot Within c:\inetpub\wwwroot.
you must rename folder to osTicket from there you need to enable php_imap.dll  php_intl.dll  php_opcache.dll

</p>
<br />

   <img src="https://i.imgur.com/jAf2qEF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



once you refresh the osticket site you need to rename ost-sampleconfig.php to ost-config.php.Then set the Permissions.Go to properties then security then advance
from there Disable inheritance then Remove All then add New Permissions to Everyone to All so everyone has permissions to do anything to the file




  <img src="https://i.imgur.com/mzfNcvd.png " height="80%" width="80%" alt="Disk Sanitization Steps"/>




Continue Setting up osTicket in the browser under help desk give it a name then create a Default email then a username and a password
before finishing download and install HeidiSQL, once finish use the user name and password from before then create a create a database called “osTicket”




 <img src= "https://i.imgur.com/mwjOTas.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>




<img src= "https://i.imgur.com/wnj7an4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<img src= "https://i.imgur.com/AFKrYXT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Congratulations, hopefully it is installed with no errors! the final step is the clean by deleting the setup folder C:\inetpub\wwwroot\osTicket\setup
once done inside root you must reset permission to read only by going to properties advance  then security now the set is done 
