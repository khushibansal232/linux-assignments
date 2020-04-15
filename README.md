# linux-assignments

1) change the Umask value for any user permanently.
Ans.  Change the umask value in following files
Root:- /etc/profile.f
Other users:- /etc/bashrc
And current user:-. /.bashrc 

2)  add a new user  without using adduser & useradd command
ans. make entry of user in followiing files
/etc/passwd
/etc/groups
make a directory for a user in /home
passwd username

3) Can we change the Umask value to 0888.
If yes, then how. If no then why ?
Ans No, beacuse Out of range

4)  how to add a new user with a Unique user id (e.g 1345) & check out the unique Id of that user.
Ans. Useradd -u <username> <id>

5) How to change the group of any folder
Ans. Chgrp <groupname> <foldername>
   
   5(a) After this checkout the group name of the files present in that folder.
Ans Cd <foldername>
          Ls -lh

   5(b)  Try to change the group of the folder & the files present in the same folder using a single command
Ans. Chgrp -R <folder name>
