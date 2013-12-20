Managing users
--------------
`sudo adduser <username>`
`sudo userdel <username>`
`sudo passwd <username>`

Display users
-------------
`/etc/passwd`

Switching to super user
-----------------------
`sudo su` CTRL+D to quit

Changing file ownership and group assignment
---------------------------------------------
* `sudo chown <owner> <file>` Change ownership to owner of the given file
* `sudo chgrp <group> <file>` Change ownership to group of the given file
* `sudo chown <owner>:<group> <file>` Change ownership to owner/group of the given file

Changing file permissions
-------------------------
`sudo chmod [g|o|u|a][+|-]<permission> <file>`

Managing processes
------------------
`top` View a list of processes  
`kill <pid>` Kill the given process by id  
`killall <command>` Kill all of the processes for the given command name

File compression and archiving
------------------------------
`tar -cvz|jf <filename>` Create a tar file with gzip(z), or bzip(j) compression  
`tar -xvz|jf <filename>` Extract a tar file  
`tar -tzf <filename>` List contents of tar file

Setting static ip
-----------------
1. Create backup of **/etc/network/interfaces**
2. Modify the file as follows:
    iface eth0 inet static
        address 192.168.A.N
        netmask 255.255.255.0
        broadcast 192.168.A.255
        network 192.168.A.0
        gateway 192.168.A.1
3. Save the file and restart the OS


tags: linux, users, owner, group, permissions, processes, tar, static ip 
