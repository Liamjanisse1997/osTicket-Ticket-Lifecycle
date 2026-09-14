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

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

Ticket 1 — Online Banking Down
1. Create the ticket as an end-user:
2. Log in as an end-user, create a new ticket, and enter “entire mobile/online banking system is down” as the issue.
3. Observe the ticket properties as john:
4. Log in to the Agent Panel as john, open the ticket, and review its Priority, Department, SLA, and Assigned To fields without changing them.



Set the ticket properties:
1. Change the ticket’s Priority to Sev-A (1 hour, 24/7) and Department to Online Banking Department; save the changes.
2. Attempt to observe/change the ticket again as john:
3. Switch back to john and reopen the ticket to see whether he can still view or modify it after the department change. The ticket should become inaccessible or restricted if john does not have access to the Online Banking Department.
4. Work the ticket to completion as jane:
5. Log in as jane, who has access to the appropriate department, open the ticket, respond to the user, document the resolution, and change the ticket status to Closed/Solved.



Ticket 2 — Adobe Upgrade
1.Create the ticket as an end-user:
2. Log in as an end-user and create a ticket stating “accounting department needs adobe upgrade, broken.”
3. Observe the ticket properties as john:
4. As john in the Agent Panel, open the ticket and record the current Priority, Department, SLA, and Assigned To values.
5. Set the ticket properties:
6. Set the ticket to Sev-B (4 hours, 24/7) and assign it to the Support department, then save the changes.
7. Work the ticket to completion as john:
As john, troubleshoot or document the Adobe upgrade issue, communicate the resolution to the end-user, and mark the ticket Closed/Solved when finished.



Ticket 3 — CFO Laptop
The ticket as an end-user:
1. Create a new end-user ticket with the issue “CFO’s laptop will no longer turn on.”
Observe the ticket properties as john:
2. Log in as john and open the ticket to review its Priority, Department, SLA, and Assigned To information.
3. Set the ticket properties:
Change the ticket to Sev-B (4 hours, 24/7) and assign it to the Support department, then save the ticket.
4. Work the ticket to completion as john:
5. As john, troubleshoot the laptop issue or document the required repair/escalation, communicate with the user, and mark the ticket Closed/Solved after resolution.



Escalating All Tickets
1. Set properties to all tickets:
Update all tickets to Sev-A, completing the SysAdmins ticket last, so you can observe how the department permissions affect access after escalation.
2. Observe the escalated ticket:
Switch to the Admin Panel, give yourself View access to Sys Admins, then return to the Agent Panel and open the escalated ticket to verify that you can now see it.
3. Observe that you cannot make changes:
Confirm that although you can view the SysAdmins ticket, you do not have the necessary permissions to modify or update it.
4. Solve all tickets:
Work through each remaining ticket, provide/document the appropriate resolution, communicate the outcome to the requester, and mark each ticket as Solved/Closed.
5. Explain ticket email capability:
Most ticketing systems, including osTicket, can send email notifications whenever a ticket is created or updated, allowing the end-user to receive the response and reply directly to the ticket.
