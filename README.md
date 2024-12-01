<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10 Pro</b> (22H2) at least 2vCPUs, 8GB RAM

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Working through Tickets</h2>

<p>
In this project, we'll simulate some helpdesk tickets and work through them to resolution. Before we start anything, make sure the Maintenance department is deleted as tickets somehow get routed here. Login as an admin,
hover over agents (big tab) and click on departments. Check the Maintenance department, click More then delete. Now we can begin.

Go to http://localhost/osTicket and open a new ticket. Let's create a ticket about a user named Karen and is reporting that their company's mobile/online banking system is down.
</p>
<br />

<p>
<img src="https://i.imgur.com/9dAEYSg.png" height="80%" width="80%" alt="user portal"/>
</p>
<p>

<img src="https://i.imgur.com/SFILH0y.png" height="80%" width="80%" alt="ticket 1 created"/>
</p>
<p>
 We will try and access this ticket with the John Doe user we created in the Post-Installation project https://github.com/jttn90/post-install-config. Looks like we can assign this ticket to others can set the SLA.
Online banking being down for a company needs to be looked at urgently so we can set the SLA to Sev-A. Although John could probably resolve this ticket since he's part of the support team, it is more appropriate
to assign this to the Online Banking team. Then Jane from the Online Banking team and work the ticket to resolution and close the ticket.
</p>
<br />
<p>
<img src="https://i.imgur.com/EmZtE25.png" height="80%" width="80%" alt="john accessing ticket"/>
<img src="https://i.imgur.com/sKLV7cd.png" height="80%" width="80%" alt="jane closing ticket"/>
</p>

<p>
Let's say in another example a ticket is created saying that the Adobe software update is broken in the accounting department. John picks up the ticket and reads through it. The ticket is a bit vague and doesn't specify whether this issue affects the entire department or whether just a 
few users are affected. We also don't know if the update is due to a faulty patch or Adobe itself. It's best to call the customer up in these cases and verify some details before working through the ticket. However, in this case we'll assume that only a few users were affected. In this case, we
set the SLA to Sev-C as it has minor impact on the business as a whole and can respond to the user to try restarting the computers and see if it works. If this actions resolves the problem, we can then close the ticket.

</p>
<img src="https://i.imgur.com/P40520h.png" height="80%" width="80%" alt="closed 2nd ticket"/>
<br />

<p>
Now for one final example, let's say the CFO of a company is unable to turn on his laptop. This can be quite serious if the CFO is unable to access critical documents for the business. However the issue may not be
  as bad as it seems depending on how fast the laptop can be fixed for eg. bad battery (easy fix) vs failed inverter (harder fix). Let's set the priority level to emergency for now and say we may change this once we
  get more information.
</p>
<br />

<p>
<img src="https://i.imgur.com/qeaz3s2.png" height="80%" width"80%" alt="closed 3rd ticket"/>
</p>
<br />
<p>
After getting more information, it turns out the charger was broken so this is a relatively easy fix, we can set the SLA to Sev-B and once we get someone to find a new charger and verify that the laptop can be
  powered on, we can close the ticket.
  
</p>

<p>
Working through tickets takes a bit digging but asking the right questions and knowing who to escalate the ticket to can help immensely.
</p>
