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
Go to Control Panel/ Programs/ Programs and Features/ Turn Windows features on or off. Then, once we get to this screen, we choose .NET Framework 3.5 and Internet Information Services. Once we go to the IIS screen, expand it and go under World Wide Web Services/ Aplication Development Features/ CGI and check it. Once all done, hit apply and ok
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


Now we are going to run IIS as an ADMIN and then go to PHP Manager, register a new PHP version, click the 3 dots, and find the PHP on the C drive (the one we made earlier). Click "php.cgi" and ok. Then go ahead and stop and start the server
</p>
<br />
<h3> Step 7. </h3>

<img width="776" height="594" alt="Screenshot 2026-08-12 at 3 37 09 PM" src="https://github.com/user-attachments/assets/456680f8-6cfe-44b6-9f91-448610df84ab" />

<img width="333" height="266" alt="Screenshot 2026-08-12 at 3 36 54 PM" src="https://github.com/user-attachments/assets/24ad4c05-eb23-4f1e-9fb4-9a65d2c25e23" />

<img width="286" height="227" alt="Screenshot 2026-08-12 at 3 39 52 PM" src="https://github.com/user-attachments/assets/4069d0d6-840d-4d8a-858e-c1c607746857" />

<img width="1118" height="655" alt="Screenshot 2026-08-12 at 3 31 41 PM" src="https://github.com/user-attachments/assets/7c785ddd-8129-429a-9f81-230549fa091b" />

Now we are going to extract the osTicket ZIP. Once it's all done, we are going to copy the "upload" folder to C:Drive/ inetpub/ wwwroot, and paste it there, renaming it "osTicket," and then go ahead and stop and start the server again.
</p>
<br />
<h3> Step 8. </h3>

<img width="385" height="448" alt="Screenshot 2026-08-12 at 3 46 01 PM" src="https://github.com/user-attachments/assets/5b5a6b60-80ee-43bf-bc79-43ad4546e426" />

<img width="396" height="315" alt="Screenshot 2026-08-12 at 3 52 21 PM" src="https://github.com/user-attachments/assets/2402b881-64a1-45a4-9676-06330dae62ca" />

<img width="380" height="376" alt="Screenshot 2026-08-12 at 3 54 09 PM" src="https://github.com/user-attachments/assets/24eab95e-4451-4785-b3c9-daebaf6dc3e6" />

Now we can load up the osTicket website, and it should load up this screen. We are now going to have to go back into IIS to make some changes so osTicket can fully run. Go to osticket-vm/sites/osTicket/PHP Manager. Enable or disable an extension. Once we get to that screen, enable these 3: "php_imap.dll," "php_intl.dll", and "php_opcache.dll." Click Apply and ok
</p>
<br />
<h3> Step 9. </h3>

<img width="668" height="780" alt="Screenshot 2026-08-12 at 4 00 35 PM" src="https://github.com/user-attachments/assets/0b9a24b9-42e0-4558-b775-89e69e5fc1dc" />

<img width="667" height="775" alt="Screenshot 2026-08-12 at 4 02 20 PM" src="https://github.com/user-attachments/assets/92198286-6310-4009-8b0b-bc22659a9f4c" />

<img width="557" height="375" alt="Screenshot 2026-08-12 at 4 07 53 PM" src="https://github.com/user-attachments/assets/cc133ed0-51e9-41aa-9ada-3164121ef3d7" />

We are now going to rename a file to give permissions. To do that, we need to go to C:Drive/ inetpub/osTicket/include/ost-sampleconfig.php. We are going to change the file name from "ost-sampleconfig.php" to "ost-config.php" and then assign permissions to everyone by clicking Properties/Security/Advanced/Disable Inheritance and add permission, hit Apply and ok
</p>
<br />
<h3> Step 10. </h3>
<img width="380" height="376" alt="Screenshot 2026-08-12 at 3 54 09 PM" src="https://github.com/user-attachments/assets/daa76b53-3b11-465e-957c-79520b46e4d1" />

<img width="667" height="781" alt="Screenshot 2026-08-12 at 4 09 36 PM" src="https://github.com/user-attachments/assets/7377087f-e776-4682-81c3-24277746e5c3" />

Hit Continue and Sign up
</p>
<br />
<h3> Step 11. </h3>


