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

Step 3: Identfy Hidden Files

I inspected the project directory for hidden files by displaying all files and folders, including those that are normally concealed from standard directory listings. This helped ensure no important configuration or project files were overlooked during the permission review process.

Command Used: 

ls -la

<img width="817" height="322" alt="Screenshot 2026-06-09 104951" src="https://github.com/user-attachments/assets/86e99ba4-4200-4132-82fe-ea7fbaa7589c" />



Purpose:

- Display all files, including hidden files.
- Review permissions and ownership of hidden resources.
- Identify files that may require security review or permission changes.

# Change File Permissions

In this task, I reviewed file permissions to identify any files with improper access settings. After locating files that granted unnecessary write permissions, I updated the permissions to restrict unauthorized access and improve overall system security.

Step 1: Identify Insecure File Permissions

Reviewed the permissions of files within the projects directory to determine whether any files granted unauthorized write access to other users.

The command to complete this step:

ls -l

<img width="852" height="268" alt="Screenshot 2026-06-09 105122" src="https://github.com/user-attachments/assets/4556bdfe-6adc-4762-9c3c-b980f95e2d34" />

Step 2: Remove Unauthorized Write Access

Modified the permissions of the identified file to remove write access for other users and reduce the risk of unauthorized changes.

The command to complete this step:

chmod o-w project_k.txt

<img width="891" height="268" alt="Screenshot 2026-06-09 123353" src="https://github.com/user-attachments/assets/00ddb1d0-62b6-4def-b027-d7088e1570a0" />

Step 3: Review Restricted File Permissions

Inspected the permissions assigned to a restricted file to verify whether group members had unnecessary read or write privileges.

The command to complete this step:

ls -l

<img width="827" height="273" alt="Screenshot 2026-06-09 123424" src="https://github.com/user-attachments/assets/9ae6cfe4-de96-42fd-8453-d3d695962dbf" />

Step 4: Restrict Group Access

Updated the file’s permissions to remove group read and write access, ensuring that only the file owner retained access to the sensitive file.

The command to complete this step:

chmod g-r project_m.txt

<img width="873" height="173" alt="Screenshot 2026-06-09 105441" src="https://github.com/user-attachments/assets/0a1567b6-9a92-4b9b-a4ae-7656cf61c573" />

Purpose:
To identify and correct improper file permissions in a Linux environment, ensuring that only authorized users have access to sensitive files and directories.

# Change file permissions on a hidden file

This task involved examining a hidden file for improper permissions and updating its access controls to ensure only authorized users could access the file.

Step 1: Review Hidden File Permissions

Listed all files, including hidden files, and examined the permissions assigned to the hidden file .project_x.txt to identify excessive write access.

The command to complete this step:

ls -la

<img width="827" height="237" alt="Screenshot 2026-06-09 105528" src="https://github.com/user-attachments/assets/1952ce4b-5208-4de5-bd7b-d88b6521fd70" />


Step 2: Restrict Unauthorized Write Access

Modified the permissions of .project_x.txt by removing unnecessary write privileges while maintaining the required read access for authorized users.

The command to complete this step:

chmod u-w,g-w,g+r .project_x.txt

<img width="815" height="251" alt="Screenshot 2026-06-09 105754" src="https://github.com/user-attachments/assets/f061dc7a-cd3d-4970-807f-80d1f9ee1788" />

Purpose: 

To audit and modify hidden file permissions to ensure that only authorized users retained the appropriate level of access.



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

