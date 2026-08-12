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

- Microsoft Azure Virtual Machine
- Remote Desktop Connection
- Internet Information Services (IIS) with CGI
- PHP and PHP Manager for IIS
- MySQL and HeidiSQL

<h2>Installation Steps</h2>
<h3> Step 1. </h3>
<p>
<img <img width="1511" height="848" alt="image" src="https://github.com/user-attachments/assets/6afbeda7-d4b5-4ca5-ae41-01bceaedc2a8" />
</p>
<p>
<p>
<img <img width="1169" height="711" alt="Screenshot 2026-08-12 at 1 40 19 PM" src="https://github.com/user-attachments/assets/49c9bcd6-28e0-4577-ae23-aaadcaff7495" />
</p>
<p>
I started off by creating a "Virtual Machine" by going to the search bar and searching for "VM." I then go to the drop box and click "Virtual Machine" and name it "osticket-vm" in Microsoft Azure. The VM runs Windows 10 and was accessed through Remote Desktop to begin the osTicket installation. I then go and put the IP address along with the username and password and log in.
</p>
<br />
<h3> Step 2. </h3>
<p>
<img <img width="1503" height="940" alt="Screenshot 2026-08-12 at 2 36 00 PM" src="https://github.com/user-attachments/assets/37178c72-6135-4784-a744-c6f2d4d4a273" />
</p>
<p>
<p>
Next, we are going to install the osTicket software and unzip the files onto your desktop. Once that's all done, we are going to configure some settings in order for osTicket to be able to run.
</p>
</p>
<br />
<h3> Step 3. </h3>
<p>
<img width="1502" height="906" alt="Screenshot 2026-08-12 at 3 03 51 PM" src="https://github.com/user-attachments/assets/53d7ad3b-df95-4fb8-aff4-f997c3fe1e38" />
<p>
<p>
Go to Control Panel/ Programs/ Programs and Features/ Turn Windows features on or off. Then, once we get to this screen, we choose .NET Framework 3.5 and Internet Information Services. Once we go to the IIS screen, expand it and go under World Wide Web Services/ Aplication Development Features/ CGI and check it. Once all done hit apply and ok
</p>
<br />
<h3> Step 4. </h3>

<img width="942" height="900" alt="Screenshot 2026-08-12 at 3 06 34 PM" src="https://github.com/user-attachments/assets/ef88d0b0-6c93-40a9-ab87-cabfe44f13f1" />

We should be able to load up the page "127.0.0.1," and it should be active; we can now proceed with the installation part
</p>
<br />
<h3> Step 5. </h3>

<img width="1510" height="909" alt="Screenshot 2026-08-12 at 3 11 23 PM" src="https://github.com/user-attachments/assets/fea28d0e-fa12-4160-aa58-984dbc8ed67a" />
<img width="780" height="606" alt="Screenshot 2026-08-12 at 3 18 29 PM" src="https://github.com/user-attachments/assets/540e87b8-2872-40c8-af61-9998d07cfa71" />
<img width="214" height="162" alt="Screenshot 2026-08-12 at 3 16 38 PM" src="https://github.com/user-attachments/assets/0f7d5aa4-505f-490c-a067-03325b7be524" />


Make a file on your C drive and name it "PHP". Extract the existing PHP file on the C drive and continue with the rest of the installation. Once you are all done with that, we are going to install SQL, click on it and go through the prompts, make sure to click on standard configurations and continue the setup as normal
</p>
<br />
<h3> Step 6. </h3>

<img width="1508" height="915" alt="Screenshot 2026-08-12 at 3 30 22 PM" src="https://github.com/user-attachments/assets/eb6e68a3-0d9f-4ce9-accd-e1fe9fd33a88" />

<img width="393" height="383" alt="Screenshot 2026-08-12 at 3 31 11 PM" src="https://github.com/user-attachments/assets/f97f5196-5236-4165-9ace-7f5420d53fe0" />

<img width="1118" height="655" alt="Screenshot 2026-08-12 at 3 31 41 PM" src="https://github.com/user-attachments/assets/c5f32394-d979-4252-98fd-45e9ca6ffbda" />


Now we are going to run IIS as an ADMIN and then go to PHP Manager, register a new PHP version, click the 3 dots, and find the PHP on the C drive (the one we made earlier), Click "php.cgi" and ok. Then go ahead and Stop and Start the server
