<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket inside AZure VM (Virtual Machine)
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
 <img width="405" height="170" alt="01_ticket1_create_end_user" src="https://github.com/user-attachments/assets/23b86282-9647-4d09-b1f2-aa2759fee84c" />

2. Log in as an end-user, create a new ticket, and enter “entire mobile/online banking system is down” as the issue.
 <img width="405" height="115" alt="02_ticket1_observe_john" src="https://github.com/user-attachments/assets/fa41c7be-d967-4c6c-b74b-51eb29ff03a9" />

3. Observe the ticket properties as john:
 <img width="405" height="145" alt="03_ticket1_set_properties" src="https://github.com/user-attachments/assets/3e280d27-3455-4dca-8305-d098ee088a88" />

5. Log in to the Agent Panel as john, open the ticket, and review its Priority, Department, SLA, and Assigned To fields without changing them.
 <img width="405" height="75" alt="04_ticket1_access_denied_john" src="https://github.com/user-attachments/assets/766a9a80-c7b1-4d9e-bf0d-f5e19534a8dd" />





Set the ticket properties:

1. Change the ticket’s Priority to Sev-A (1 hour, 24/7) and Department to Online Banking Department; save the changes.
 <img width="410" height="145" alt="08_ticket2_set_properties" src="https://github.com/user-attachments/assets/57b52102-5c9f-47d0-b3cf-bd3a698c314a" />

2. Attempt to observe/change the ticket again as john:
 <img width="410" height="115" alt="11_ticket3_observe_john" src="https://github.com/user-attachments/assets/5a50290d-a2b2-4acd-90eb-3e2eb080f604" />

3. Switch back to john and reopen the ticket to see whether he can still view or modify it after the department change. The ticket should become inaccessible or restricted if john does not have access to the Online Banking Department.
 <img width="405" height="75" alt="04_ticket1_access_denied_john" src="https://github.com/user-attachments/assets/d3f20dbb-3b84-4924-9fec-ecec66a0e052" />

4. Work the ticket to completion as jane:
5. Log in as jane, who has access to the appropriate department, open the ticket, respond to the user, document the resolution, and change the ticket status to Closed/Solved.
 <img width="405" height="110" alt="05_ticket1_complete_jane" src="https://github.com/user-attachments/assets/6d149c1c-0de5-4673-9600-d4ca2e43cddf" />




Ticket 2 — Adobe Upgrade

1. Create the ticket as an end-user:
 Log in as an end-user and create a ticket stating “accounting department needs adobe upgrade, broken.”
<img width="410" height="170" alt="10_ticket3_create_end_user" src="https://github.com/user-attachments/assets/830cc33b-b0b3-436d-a8ae-837404b65239" />

 
2. Observe the ticket properties as john:
 As john in the Agent Panel, open the ticket and record the current Priority, Department, SLA, and Assigned To values.
<img width="410" height="115" alt="07_ticket2_observe_john" src="https://github.com/user-attachments/assets/b2607ad0-a0e1-4127-ac0a-02f6f044ea2c" />


4. Set the ticket properties:
 Set the ticket to Sev-B (4 hours, 24/7) and assign it to the Support department, then save the changes.
<img width="410" height="145" alt="12_ticket3_set_properties" src="https://github.com/user-attachments/assets/f4d2b157-9e1f-4308-91d3-0808f70bbc32" />


6. Work the ticket to completion as john:
As john, troubleshoot or document the Adobe upgrade issue, communicate the resolution to the end-user, and mark the ticket Closed/Solved when finished.
<img width="410" height="140" alt="09_ticket2_complete_john" src="https://github.com/user-attachments/assets/23c729e1-296f-4677-a66b-8513cbd2e6cd" />





Escalating All Tickets
1. Set properties to all tickets:
Update all tickets to Sev-A, completing the SysAdmins ticket last, so you can observe how the department permissions affect access after escalation.
<img width="205" height="220" alt="14_escalation_set_all_seva" src="https://github.com/user-attachments/assets/85a46d21-bb61-42dd-9432-10f1a2855698" />

2.. Observe the escalated ticket:
Switch to the Admin Panel, give yourself View access to Sys Admins, then return to the Agent Panel and open the escalated ticket to verify that you can now see it.
<img width="210" height="220" alt="15_escalation_admin_view_sysadmins" src="https://github.com/user-attachments/assets/62b0aff2-f827-4838-be09-ae0cc8852124" />

3.Observe that you cannot make changes:
Confirm that although you can view the SysAdmins ticket, you do not have the necessary permissions to modify or update it.
<img width="205" height="220" alt="17_escalation_cannot_make_changes" src="https://github.com/user-attachments/assets/70fb6daa-6c0e-412a-ab63-fd8bb5af7c7a" />

4. Solve all tickets:
Work through each remaining ticket, provide/document the appropriate resolution, communicate the outcome to the requester, and mark each ticket as Solved/Closed.
<img width="210" height="220" alt="18_solve_all_tickets" src="https://github.com/user-attachments/assets/e2ef7faf-eacf-4405-aae2-b93e2cf46dd9" />

5. Explain ticket email capability:
Most ticketing systems, including osTicket, can send email notifications whenever a ticket is created or updated, allowing the end-user to receive the response and reply directly to the ticket.
<img width="200" height="220" alt="19_email_capability" src="https://github.com/user-attachments/assets/027b7344-0169-49c6-ac74-51d507113a14" />
