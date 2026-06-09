# User & Permission Management
## Project Overview

This project demonstrates how Linux file permissions and ownership settings can be configured to enforce access control and reduce security risks.

## Project Objective

Review and modify file permissions to ensure users have only the access required to perform their job functions.

## Technologies Used

- Linux
- Bash
- chmod
- File Permissions

## Examine Current Permissions

Used ls -la to review file and directory permissions.

## Restrict Access

Used chmod to remove unnecessary permissions.

## Verify Changes

Confirmed permissions matched security requirements.

# Check file and directory details

I began by reviewing the contents and permissions of the project directory. This allowed me to identify existing access settings and determine which files or directories required permission changes.

Step 1: Navigate to the Project Directory

I accessed the projects directory, which contained the files and folders assigned to the researcher2 user.

Command Used:

cd projects

<img width="676" height="353" alt="Screenshot 2026-06-09 115006" src="https://github.com/user-attachments/assets/ac325345-cdaa-4331-a1d0-4a0224b240ca" />

Step 2: Review Directory Contents and Permissions

I listed the contents of the directory and examined the associated permissions for each file and folder. This provided visibility into current access rights before making any modifications.



Command Used: 

ls -l

<img width="945" height="362" alt="Screenshot 2026-06-09 104850" src="https://github.com/user-attachments/assets/aeb946c6-39bd-41d5-bd16-e7d644d00254" />

Purpose:

- View files and directories within the project folder.
- Examine ownership and permission settings.
- Identify files that may require permission adjustments.









## Findings

- Identified files with excessive permissions.
- Restricted unauthorized access.
- Applied the principle of least privilege.
- Improved system security through access control.

## Skills Demonstrated

- Linux Administration
- Access Control
- Security Hardening
- User Management
- Principle of Least Privilege

## Conclusion

This project demonstrated how Linux permissions can be used to secure sensitive files and ensure access is limited to authorized users.

