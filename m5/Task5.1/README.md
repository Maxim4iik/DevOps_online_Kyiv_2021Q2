# DevOps_online_Kyiv_2021Q2

1.2) 		/etc/passwd

1.3) 		cat /etc/passwd   имя_пользователя пароль ид ид_группы группа домашний_каталог оболочка

Photo Task1.4

1.6)		sudo cat .bash*

Photo Task1.7

Photo Task1.8

/bin – Essential User Binaries
/boot – Static Boot Files
/cdrom – Historical Mount Point for CD-ROMs
/dev – Device Files
/etc – Configuration Files
/home – Home Folders
/lib – Essential Shared Libraries
/lost+found – Recovered Files
/media – Removable Media
/mnt – Temporary Mount Points
/opt – Optional Packages
/proc – Kernel & Process Files
/root – Root Home Directory
/run – Application State Files
/sbin – System Administration Binaries
/srv – Service Data
/tmp – Temporary Files
/usr – User Binaries & Read-Only Data
/var – Variable Data Files

Photo Task2.1

Photo Task2.2

Photo Task2.3
The relative path begins with a dot (period), representing the current directory. The relative path is valid only if the current directory contains a path named like the file which contains a directory named ‘name-of-directory’.

2.4)
File list: one file per line
ls -1
File list: all files(including hidden)
ls -a

Photo Task2.10

Photo Task2.11

2.13)
ls -l /dev. 
The first bit on each line. Device files are denoted as the following:
	•	c - character
	•	b - block
	•	p - pipe
	•	s - socket
Character Device
These devices transfer data, but one a character at a time. You'll see a lot of pseudo devices (/dev/null) as character devices, these devices aren't really physically connected to the machine, but they allow the operating system greater functionality.
Block Device
These devices transfer data, but in large fixed-sized blocks. You'll most commonly see devices that utilize data blocks as block devices, such as harddrives, filesystems, etc.
Pipe Device
Named pipes allow two or more processes to communicate with each other, these are similar to character devices, but instead of having output sent to a device, it's sent to another process.
Socket Device
Socket devices facilitate communication between processes, similar to pipe devices but they can communicate with many processes at once.

2.14)
  -     Regular File  
d      Directory   
l       Link File    
c      Character Device File 
s      Local Socket File  
p      Named Pipe File    
b      Block Device File   
