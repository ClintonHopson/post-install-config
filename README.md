# post-install-config
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>
- Configure HediSQL database for the ticket system
- Set up Roles
- Set up Departments 
- Assign Agents to different teams
- Set up agents ( for the sake of working the system )
- Set SLA's 

<h2>Configuration Steps</h2>

Ok great you have installed osTicket but we still have a bit to do before we are in the system and logged on we have to make users / Admins to login as. 
1ST fill in the (system settings) and( admin user info )

![Ok great you have installed osTicket but we still have a bit to do…](https://github.com/user-attachments/assets/1a926c6b-596e-4770-9b8d-37a2720ad2d0)

2nd Go back to your osTicket install folder and double click and install ( HeidiSQL_12.3.0.6589_Setup). 
![Ok great you have installed osTicket but we still have a bit to do…](https://github.com/user-attachments/assets/6659730d-314f-4765-9f2c-5f46d07aa8d3)


3rd : Once HeidiSQL is installed you will Select “ New “ then enter  “ root “ in the user and password sections this will connect us to our osTicket database so we can add users , Admins , SLA’s etc…

![Ok great you have installed osTicket but we still have a bit to do…](https://github.com/user-attachments/assets/043d9dea-8ae0-403f-9fb4-c90edad17f13)

4th Once you are conected right click on Unnamed > database > rename it to “osTicket” and save 

![Ok great you have installed osTicket but we still have a bit to do…](https://github.com/user-attachments/assets/84b8c912-0301-49b4-8b39-ddda4aaa3299)

5th Now go back to the osTicket brower scroll down to database settings and enter “ osTicket “ in the ( MySQL Database: ) and enter the root user and password then select “ install “  
![Ok great you have installed osTicket but we still have a bit to do…](https://github.com/user-attachments/assets/7c41bd73-9cca-4e0b-9fd7-5c63b4d7f554)

