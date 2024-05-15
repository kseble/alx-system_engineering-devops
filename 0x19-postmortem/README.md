
0x19. Postmortem An ALX - Software Engineering Task

The Puzzle
Write a post-mortem for a technical coding project with the following Requirements:
- Issue Summary (that is often what executives will read) must contain: - duration of the outage with start and end times (including timezone) - what was the impact (what service was down/slow? What were user experiencing? How many % of the users were affected?) - what was the root cause
- Timeline (format bullet point, format: time - keep it short, 1 or 2 sentences) must contain:- when was the issue detected- how was the issue detected (monitoring alert, an engineer noticed something, a customer complained)- actions taken (what parts of the system were investigated, what were the assumption on the root cause of the issue)- misleading investigation/debugging paths that were taken- which team/individuals was the incident escalated tohow the incident was resolved
- Root cause and resolution must contain:- explain in detail what was causing the issue- explain in detail how the issue was fixed
- Corrective and preventative measures must contain:- what are the things that can be improved/fixed (broadly speaking)- a list of tasks to address the issue (be very specific, like a TODO, example: patch Nginx server, add monitoring on server memory


Issue Summary:
March 16, 2024 01:00 local time (22:00 GMT) CBE bank app experienced a glitch which allowed several users to withdraw money they didnt have. This caused the bank to lose millions of ETB.


Impact:
Due to the glitch that occured a lot of money was withdrawn by customers who accessed the mobile app and ATM machine.


Root Cause:
The root cause of the error was problem which occured while trying to update the system. There was some framework problem which caused the glitch.


Timeline:
- 01:20 AM  The operations team attempted to update the system
- 01:30 AM  The issue was first detected by monitoring system, which sent out an alert to the operations team.
- 01:40 AM  The team began investigating the issue, assuming it was a problem with the servers configuration.
- 02:00 AM  Further investigation revealed that users were withdrawing money they didnt have.
- 3:15 AM  The team started looking into the code to identify any potential causes of the glitch.
- 3:45 AM  The team identified the glitch in the code and began working on a fix.
- 6:30 AM  The team deployed the fix and restarted the web server.
- 7:45 AM  The system was back online and fully operational.


Misleading Investigation/Debugging Paths:
The team initially assumed that the problem was related to the cybersecurity attack and invested valuable time investigating. This delayed determining the true cause of the problem.


Incident Escalation:
The incident was initially assumed to be cybersecurity attack when the root cause was know to be a glitch during system update, it was handled promptly.


Resolution:
A Glitch on system was identified during updating a mobile banking system which make the bank lose millions. after the main cause was known, it was fixed.


Corrective and Preventative Measures:
To prevent similar issues in the future, we will implement the following corrective and preventative measures:
- Be cautious when updating system 
- Implement more robust monitoring of server performance and resource usage.
- Improve documentation and training for the operations team to better handle incidents like this in the future.


Specific tasks to address the issue include:
- Conduct a comprehensive review of the update.
- Implement additional automated tests to detect any glitchs.

