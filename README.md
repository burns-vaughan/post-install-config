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

1. Configure roles
2. Configure departments
3. Configure teams
4. Allow anyone to create tickets
5. Configure Agent (workers)
6. Configure Users (customers)
7. Configure SLA
8. Configure Help Topics

<h2>Configuration Steps</h2>
<h3>1. Configure roles</h3>
Begin by logging into osTicket as an admin. The credentials were created in a previous step.
To log in as an admin go to the following website:

http://localhost/osTicket/scp/login.php  <br>
Once you log in you will see the admin panel.

It's worth point out that there are two accounts you have access to after log in. The Agent user interface, and the Admin user interface. You switch between them using the option at the top right the screen.

For the following steps we will be configuring a bunch of settings and should be done using the Admin user interface.

Next we will create a supreme admin. Go to:

Agents > Roles > Add new role

Name is something convenient like supreme admin

Give it access to everything in the next screen. And click ok and next.

<h3>2. Configure departments</h3>

Create a new department by clicking on departments near the top of the screen. After that, create one called System Admins.

<h3>3. Configure teams</h3>

Create a new team, that is named Help Desk Support II

<h3>4. Allow anyone to create tickets</h3>

Go into the settings and tick the box that only allows users who are registered to create tickets.

It's under Settings > Users

<h3>5. Configure Agent (workers)</h3>

These are accounts that are for support agents. However, we will be create 'dummy' accounts with generic info. The main thing is to note down the username and password to use them.

<h3>6. Configure Users (customers)</h3>

Now, we will add some 'dummy' customers. These are people that have issues and submit tickets for the agents above to solve. Create a few dummy accounts.

<h3>7. Configure SLA</h3>

Go to Manage > SLA and create some generic SLA's

Such as SEV-A for high a business critical SLA. Give them some reasonable timeframes. Some common ones are:
A (1 hour, 24/7)
B (4 hours, 24/7)
C (8 hours, business hours)


<h3>8. Configure Help Topics</h3>

Create help topics for the common issues. They can be anything but some common ones are:

- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset

Your osTicket is now completely set up!

