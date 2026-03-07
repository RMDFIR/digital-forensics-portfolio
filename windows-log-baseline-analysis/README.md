# Windows Event Log Analysis – Login Activity

## Objective
To understand normal Windows login behavior and identify differences between successful and failed login attempts.

## Environment
- Windows 11 Virtual Machine
- Local user account
- Windows Event Viewer
- Security Log

## Investigation Process
1. Filtered Security log for Event ID 4624 (successful logons)
2. Filtered Security log for Event ID 4625 (failed logons)
3. Generated controlled failed login attempts
4. Compared fields including Logon Type, Account Name, and Failure Reason
5. Bonus: Filtered Security log for Event ID 4672 (Privilege List)

## Findings
- Successful logons commonly displayed Logon Type 2 (Interactive)
- Failed logons included specific failure reasons
- Local account activity did not include remote source IP addresses

## Analysis
Understanding baseline login behavior is critical for identifying abnormal authentication activity such as brute-force attempts or unauthorized access.

## Lessons Learned
- Learned how to filter Security logs efficiently
- Improved comfort navigating high-volume logs
- Identified key fields relevant to authentication investigations

## Skills Demonstrated
- Log filtering and analysis
- Pattern recognition
- Structured documentation
- Investigative reasoning

## Screenshots
Example filtered Event Viewer results showing successful login events (4624)
- <img width="830" height="548" alt="image" src="https://github.com/user-attachments/assets/ad67b329-f8c0-46c7-a0c8-7b854fd82b16" />

Example filtered Event Viewer results showing failed login events (4625)
- <img width="838" height="359" alt="image" src="https://github.com/user-attachments/assets/072c1026-8a6a-452e-b871-3721de745b27" />

Example filtered Event Viewer XML details showing PrivilegeList (4672)
- <img width="975" height="444" alt="image" src="https://github.com/user-attachments/assets/1f3b7f26-e99b-4c29-8401-03f38c56d809" />

