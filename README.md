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
<a href="https://imgur.com/IUp0f54"><img src="https://i.imgur.com/IUp0f54.png" title="source: imgur.com" /></a>

<p>
Begin setup by first signing in as Admin through the Agent sign-in otption of osTicket. 
</p>

<a href="https://imgur.com/b9wT4Kc"><img src="https://i.imgur.com/b9wT4Kc.png" title="source: imgur.com" /></a>

<p>Next navigate to Admin Panel on the top right of the browser and click. It will bring you to the Admin Dashboard. From there you will click on the Agents tab.</p>

<a href="https://imgur.com/x21KExb"><img src="https://i.imgur.com/x21KExb.png" title="source: imgur.com" /></a>
<p>
In the Agents tab, click on Roles and Add a New Role called "Supreme Admin" with Internal Notes of  "Anyone with this role has every permission".
</p>

<a href="https://imgur.com/FLrFJh1"><img src="https://i.imgur.com/FLrFJh1.png" title="source: imgur.com" /></a>

<p>
Next, create a new Department for System Administrators. while still in the Admin panel, click the Agents tab and click on Add New Departments to create a new Department within osTicket. Name it System Administrators. Leave the rest of the setting alone for now, and create department.
</p>

<a href="https://imgur.com/oXd6MtI"><img src="https://i.imgur.com/oXd6MtI.png" title="source: imgur.com" /></a>
<p>
While still in the Agents tab, click Add New Team and create a new Team called Level II Support. 
</p>

<a href="https://imgur.com/5LF6ttM"><img src="https://i.imgur.com/5LF6ttM.png" title="source: imgur.com" /></a>

<p> To simulate a working help desk platform, I will create several Agents. Click on Add New Agent and create the account credentials for each new agent. In this case, Jane and John Doe are created. </p>

<a href="https://imgur.com/NutxfNh"><img src="https://i.imgur.com/NutxfNh.png" title="source: imgur.com" /></a>

<p>Before creating users, we need to make sure that registration and login is required in order to create tickets. while still in the Admin Panel, click Settings > Users > check "Require registration and login to create tickets" </p>

<a href="https://imgur.com/qBScg6u"><img src="https://i.imgur.com/qBScg6u.png" title="source: imgur.com" /></a>

<p>To create new Users, navigate out of the Admin Panel and into the Agent Panel. Click the Users tab and click Add User. In this case, I created users Jack and Jill.</p>

<a href="https://imgur.com/JwBstgk"><img src="https://i.imgur.com/JwBstgk.png" title="source: imgur.com" /></a>

<p> Next Service Level Agreements (SLAs) will have to be made in order to categorize tickets according to their level of urgency. To make new SLAs, navigate back to the Admin Panel, click the Manage tab, and select SLA. Then click Add New SLA Plan. In this case, SEV-A, B, and C have been created to categorize tickets that need to be resolved within 1 hour (24/7), 4 hours (24/7), and 8 hours (Business Hours) respectively.
</p>

<a href="https://imgur.com/vWOSxtM"><img src="https://i.imgur.com/vWOSxtM.png" title="source: imgur.com" /></a>

<p>Finally, Help Topics need to be created to help users select an appropriate category that describes their problem so that Agents get an idea of what problem is described in the ticket. To make a new Help Topic, enter the Admin panel and open the Manage menu. Click on Help Topics and click on Add New Help Topic. In this case, I have added the following in order to use later for when I create new tickets to resolve: Business Critical Outage, Personal Computer Issues, Equipment Reset, and Password Request.
</p>

<br />

<h2>osTicket Configurations are Complete </h2>

Now that the configurations have been set in place, I can now utilize osTicket as a proper ticketing system. I can create tickets and be able to traige them as if I were in a real environment.
