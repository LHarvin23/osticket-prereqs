
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

- Windows 10
- IIS
- MySQL
- PHP
  

<h2>Installation Steps</h2>

<p>
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/bdeb7c9c-100c-46b6-b2b9-e8347b4018f1" />

</p>
<p>
Download the latest zip file of OsTicket 
</p>
<br />


<p>
<img width="768" height="607" alt="image" src="https://github.com/user-attachments/assets/56003d8d-9dbe-4043-9b61-4ff0ffa0b567" />

</p>
<p>
Install / Enable IIS in Windows WITH CGI
</p>
<br />


<p>
<img width="386" height="336" alt="image" src="https://github.com/user-attachments/assets/b84f1b80-25a3-4680-bd1a-d8084ec9e385" />

</p>
<p>
 install PHP Manager for IIS</p>



<p>
<img width="645" height="491" alt="image" src="https://github.com/user-attachments/assets/c539ded1-98ee-4859-a702-313653711989" />

</p>
<p>
Create the directory C:\PHP
</p>


<p>
<img width="574" height="348" alt="image" src="https://github.com/user-attachments/assets/9fb0dcba-faa3-4c67-9e7d-13ac0a29395b" />

</p>
<p>
Unzip PHP file into the “C:\PHP” folder
</p>


<p>
<img width="499" height="385" alt="image" src="https://github.com/user-attachments/assets/b161f306-e66d-4dd6-8dc6-6b3c15238b31" />


</p>
<p>
From OsTicket zip file install MySQL
</p>


<p>
<img width="760" height="328" alt="image" src="https://github.com/user-attachments/assets/2100ddd1-7208-4add-8c89-fe73fe5ec30e" />


</p>
<p>
Open IIS as an Admin, 
Register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe)
, Reload IIS (Open IIS, Stop and Start the server)

</p>


<p>
<img width="823" height="407" alt="image" src="https://github.com/user-attachments/assets/819e326d-1f6c-437f-894e-fff5ed0280d9" />


</p>
<p>
Install OsTicket from "OsTicket zip file', Reload IIS, Go to sites -> Default -> osTicket
On the right, click “Browse *:80”. 
Go back to IIS, sites -> Default -> osTicket,
Double-click PHP Manager,
Click “Enable or disable an extension”. 
Enable: php_imap.dll, php_intl.dll, php_opcache.dll.
Refresh the osTicket site in your browser, observe the changes.


<p>
<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/fa8c0f94-7c15-4bb1-9bee-a909340b6ab0" />


Download Heidi SQL. Create a new session. Connect to the session. Create a database called OsTicket </p>



<p>
<img width="868" height="667" alt="image" src="https://github.com/user-attachments/assets/775ba8e7-4293-4654-be9d-32e3ed684e54" />


</p>
<p>

Continue to setup OsTicket in browser. Create username and password in MySQL. Congradulations you have successfully created OsTicket!

