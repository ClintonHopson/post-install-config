<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket help desk logo"/>
</p>

<h1>osTicket Post-Install Configuration & Administration</h1>


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

6th if you have done everything correctly so far you will see this! 
![Ok great you have installed osTicket but we still have a bit to do…](https://github.com/user-attachments/assets/1966a090-73ce-48de-ae2b-c88364695fb8)

7th great now that you have installed and configured our data base for osTicket lets get logged in and start adding out agents and end users and setting up SLA’s Click this URL ( http://localhost/osTicket/scp/login.php ) to bring up the log in page for Users and login with your admin user and password. Also open up a new tab click thiS URL ( http://localhost/osTicket/scp/login.php ) for end users. 
![Ok great you have installed osTicket but we still have a bit to do…](https://github.com/user-attachments/assets/c74ae9df-e4e4-4ffa-9ed0-a5bf24cb2705)


8th Take notice of the difference  between the admin panel and agent panel as we will be going back and forth between these two 

Agent Panel 
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/f99be2d0-5d2c-4794-905b-fd4f2194b491)

Admin Panel
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/c6ac1049-cffb-4621-a259-92cc7c457f28)

9th now on the Admin panel we will make a “Supreme Role “ that can do everything in osTicket. 
Go to Agents > Roles > add new role
<img width="1996" height="2374" alt="image" src="https://github.com/user-attachments/assets/0a2a19d0-1873-4724-b24c-c70e8a7c765e" />

10th then select the permissions tab and check all the boxes in the “ Tickets , Tasks , and Knowledge base “ tabs then select add role
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/819768b9-6897-4514-ac2b-a84100f8e715)

11th now on the admin panel > top row “agents “ > departments select “add new department"
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/396ce266-53c0-469d-bab5-17c457e6b2f6)


12th name this new department “SysAdmins “ and select “ Top-Level-Department”, then create the department.
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/cb88bc08-4e54-4b5c-bbfc-2339c50385d9)

13th now in the admin panel, select Agents >   teams  > Add New Team 
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/73b5f8a7-5336-47be-8cda-307e5b5df3c1)

14th name this new team “ Online Banking “ and select Create Team
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/65e13ada-34da-4b04-8b5a-b933ac270f75)

15th next on the Admin Panel, go to “Settings “ top row > user settings > and make sure the box next to (require registration and login to create tickets)  is unchecked. This will allow users to make tickets without having to have an account.
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/b5257eaf-9326-41b9-aa54-c0a9c5e3df1d)

16th  now we will add users and workers to the system. Go to Admin panel > agents ( top row ) > agents ( bottom row ) > add new agent 
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/416e2d20-d01e-4ecc-a96b-9ef1a64138ff)

17th fill out Jane's info below, then go to access
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/8ad0c130-296c-4c24-9fa0-9758fdbcb18c)

18th  in access set her primary department to SysAdmins and Supreme Admin, then add her to the “ Online banking “ team in the teams tab.
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/91cfb06a-a0c8-4f8b-908f-4e067d2e261e)

19th Do the same steps  again but this time we are making John's account.Set his primary department to “ Support “ and “view only". 
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/0e677e55-0071-46f6-b175-fd089104637b)

20th Too set the Jane and John users' passwords, select “ set passwords, “ uncheck the blue bo,x and set the passwords to something you will remember or write them down
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/c1acc93b-6d2f-435c-b4b1-6007e5c4f75a)

21st  next we will add a user who can create tickets. So first go to the agent panel > users > add new and add Karen and fill out all the respective info
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/80618386-5833-4876-9f85-27ca08f88bad)

22nd next we will set up our SLA’s so go to Admin panel > manage > SLA > Add New SLA Plan 
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/6e6d5254-0882-4a8c-98d5-12bf218ab646)

23rd here we will add 3 different SLA levels proceed as follows 
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/ac00f960-b297-4655-a0e3-52a6720c5934)

24th, this is what the SLA panel should look like when finished
![13th next select create new department and Name is “ SysAdmin “ and…](https://github.com/user-attachments/assets/98b56d5e-f9ab-48ac-aa03-67ae706270bb)


Congrats, you have now set up your operating parameters for you and your team in osTicket and are ready to solve issues!


