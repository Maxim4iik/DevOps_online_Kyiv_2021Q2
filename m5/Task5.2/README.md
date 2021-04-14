# DevOps_online_Kyiv_2021Q2

1) etc/passwd   
login userid (stored in variables $USER or $LOGNAME in the shell) 
encrypted password (or an x marker indicating use of /etc/shadow)
User ID number (UID)
Group ID number (GID) - but users can be in more groups, 
tooComments: any text information; often the user’s full name and/or office
Home directory (absolute path): usually /home/$USER
Login shell to give the user at login; usually /bin/bash
etc/groups
group name
encrypted password (or an x marker indicating use of /etc/gshadow)
Group ID number (GID)
Optional list of userids that are members of that group
	•	The above information about groups is kept in /etc/group
	•	Modifications can be done by root or by the Group Administrator for a group
	•	Its content can be viewed by anyone
	•	Encrypted passwords are usually stored in /etc/gshadow, accessible only by root

2) Uid ranges (user id) - is used to determine which system resources user can access

3) GID (group id) - is a numeric value used to represent a specific group

4) Using command groups

5) useradd [OPTIONS] USERNAME

6) usermod -l login-name old-name

7) Directory /etc/skel/ is used to initiate home directory when a user is first created.

8) userdel -r user_name

9) sudo passwd -l user_name

10) passwd --expire ravi

11) ls -A -a -b -c -C -d -F -f -g -h -I -k -L -l -m -n -o -p -q -R -r -s -t -u -x

12) Read, Write, Execute. For Owner, Group, Others

13) User can make some action with file

14) chown name_of_new_owner file_name

15) example octal: "724" 
Owner Permissions - 7 = rwx
Group Permissions - 2 = -w-
Other Permissions - 4 = r--

$ chmod 777 myfile.txt 
You can then confirm the change using ls -l 
$ ls -al 

16) When a directory has the sticky bit set, its files can be deleted or renamed only by the file owner, directory owner and the root user. The command below shows how the sticky bit can be set.
	chmod +t 

17) Read-only (R) : Allows a file only to be read and not modified.
	Archive (A) : Enables windows backups.
	System (S) : Denotes the file as one that’s part of the operating system.
	Hidden (H) : Hides the file in windows explorer.
	Compressed (C) : Windows will compresses the file.
	Encrypted (E) : Windows will encrypt the file.
	Not Content-Indexed (I)
