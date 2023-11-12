# Security Symphony: File Permissions Harmony in Linux

## Background

Within the organizational tapestry, the research team plays a pivotal role, and safeguarding their digital realm is paramount. The project emerged from the need to meticulously examine and refine file permissions in designated directories, aligning them with the required authorization levels. This initiative is a linchpin for upholding the security of our system, ensuring that users on the research team have the appropriate permissions for a secure environment.

## Objectives

The primary objectives of this project are:

1. **Authorization Alignment:** Scrutinize existing file permissions, ensuring they match the required authorization levels for users on the research team.
   
2. **Security Enhancement:** Modify permissions where necessary to authorize appropriate users and remove any unauthorized access, fortifying the system's security.

## Supporting Material

Explore the [Current File Permissions document](#) to delve into the intricate details of the existing file structure and permissions. This document serves as a compass, guiding the project through the labyrinth of file permissions.

## Project Steps

1. **Check File and Directory Details:**
   - Utilize powerful Linux commands, especially 'ls -la,' to scrutinize existing permissions, revealing hidden files, directories, and their associated permissions.

   ```bash
   ls -la
   ```
2. **Describe the Permissions String:**
  - Dissect the ten-character permission string, unraveling the cryptic code that signifies access rights for users, groups, and others.

3. **Change File Permissions:**
  - Identify and modify permissions as needed, ensuring alignment with the organization's security directives. The use of 'chmod' commands orchestrates these strategic adjustments.
```bash
chmod o-w project_k.txt
```
4. **Change File Permissions on a Hidden File:**
  - Navigate the realm of concealed files, adjusting permissions to restrict and grant access as required.
```bash
chmod u-w,g-w,o-r .project_x.txt
```
5. **Change Directory Permissions:**
  - Delicately adjust permissions for specific directories, aligning them with the organization's access requirements.
```bash
chmod g-x drafts
```

## Project Conclusion
In this symphony of security, the project culminates in a meticulously sculpted landscape of file permissions within the projects directory. The adjustments, guided by a vigilant review using 'ls -la,' fortify the security posture in line with the organization's authorization mandates.

## Feedback
Your insights and feedback on this project are invaluable. Please review the detailed project steps and outcomes in the provided [GitHub repository](https://github.com/JustinAntunes-Cardoso/Linux-Permissions) and share your thoughts.

**Note**
I've independently completed this project.
