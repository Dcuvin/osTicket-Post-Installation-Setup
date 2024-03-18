<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configurations</h1>

<h2>Goal: Properly setup and configure osTicket</h2>

This lab demonstrates the necessary changes I make to configure osTicket so it can be used as a proper ticketing system.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- osTicket 

<h2>Operating Systems Used </h2>

- Windows 10 Pro</b> (21H2)


<h2>Configuration Steps</h2>

<p>
Begin setup by first signing in as Admin through the Agent sign-in otption of osTicket. 
</p>

<p>Next navigate to Admin Panel on the top right of the browser and click. It will bring you to the Admin Dashboard. From there you will click on the Agents tab.</p>

<p>
In the Agents tab, click on Roles and Add a New Role called "Supreme Admin" with Internal Notes of  "Anyone with this role has every permission".
</p>

<p>
Next, create a new Department for System Administrators. while still in the Admin panel, click the Agents tab and click on Add New Departments to create a new Department within osTicket. Name it System Administrators. Leave the rest of the setting alone for now, and create department.
</p>

<p>
While still in the Agents tab, click Add New Team and create a new Team called Level II Support. 
</p>
<p> To simulate a working help desk platform, I will create several Agents. Click on Add New Agent and create the account credentials for each new agent. In this case, Jane and John Doe are created. </p>

<p>Before creating users, we need to make sure that registration and login is required in order to create tickets. while still in the Admin Panel, click Settings > Users > check "Require registration and login to create tickets" </p>
<br />

