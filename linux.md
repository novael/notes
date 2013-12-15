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

tags: linux, users, owner, group, permissions, processes
