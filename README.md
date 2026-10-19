# Ancora-Education-Ucertify-Lab58
# Managing File Ownership and Attributes

> **Original Lab Source**
> 
> This lab was available through:
>
> [https://ancoraeducation.ucertify.com/app/?func=navigate_items&item_sequence=11]

## Objective of the Lab
In this lab, you will learn to manage file ownership and attributes. Each file and directory belongs to a specific group ID and has a set of permissions associated with it. In this lab, you will use the chown command to change the ownership for a file or group. 
## Instructions
### STEP 1
From the desktop, open the Terminal window. 
### STEP 2
Execute the following command to switch to the root account:
```bash
su -
```
### STEP 3 
Execute the following command to copy the /etc/group file to the /tmp directory:
```bash
cp /etc/group /tmp
```
### STEP 4 
Execute the following command to change the user ownership of the /tmp/group file to the student user:
```bash
chown student /tmp/group
```
### STEP 5
Execute the following command to change the group ownership of the /tmp/group file to the bin group:
```bash
chgrp bin /tmp/group
```
### STEP 6 
Execute the following command to make the /tmp/group file immutable:
```bash
chattr +i /tmp/group
```
### STEP 7 
Execute the following command to display the file attributes of the /tmp/group file:
```bash
lsattr /tmp/group
```
### STEP 8 
Execute the following command to remove the immutable attribute from the /tmp/group file:
```bash
chattr -i /tmp/group
```
### STEP 9
Execute the following command to remove the /tmp/group file:
```bash
rm /tmp/group
```
### STEP 10 
Enter yes, when permission asked for remove regular file '/tmp/group'.
## Disclaimer

This repository is for **educational and personal learning purposes only**.  

The original lab content belongs to **uCertify / Ancora Education** and remains their copyrighted material.  
This repository is not affiliated with, endorsed by, or sponsored by uCertify or Ancora Education.  

No copyright infringement is intended.  
Use of any tools or techniques mentioned here should only be performed in authorized, legal environments.
