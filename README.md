# linux-assignments

Assignment - 1
Q-1 when we create a user ,some hidden files are genrated in the directory of the same user at that time . how is it done ?
Ans  ls -a    /cmd use for to see the hidden file in linux
     . / .. it is show that folders are hidden or not.
Q-2 make subdirectories inside a parent directory by using single mkdir command .
Ans-  mkdir -p a/{a1,a2,b/c/c1}

Q-3 tac & cat cmd
Ans-  The word tac is reverse of the word cat. 
    The tac command functionality is also reverse of the cat command. 
    cat command prints the file. tac command prints the file in reverse order with the last line first


ASsignment-2
1) change the Umask value for any user permanently.
Ans.  Change the umask value in following files
For changing umask value for Root:- /etc/profile.f
For changing umask value for Other users:- /etc/bashrc
For changing umask value for current user:-. /.bashrc 

2)  add a new user  without using adduser & useradd command
Ans. Make entry of user in followiing files
/etc/passwd
/etc/groups
make a directory for a user in /home
passwd username

3) Can we change the Umask value to 0888.
If yes, then how. If no then why ?
Ans No, beacuse Out of range

4)  how to add a new user with a Unique user id (e.g 1345) & check out the unique Id of that user.
Ans. Useradd -u <username> <id>
     Useradd -u khushi 1234
5) How to change the group of any folder
Ans. Chgrp <groupname> <foldername>
     chgrp newgroup folder
   
   5(a) After this checkout the group name of the files present in that folder.
Ans Cd <foldername>
     Ls -lh

   5(b)  Try to change the group of the folder & the files present in the same folder using a single command
Ans. Chgrp -R <folder name>
