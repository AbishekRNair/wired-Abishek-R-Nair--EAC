#**Bandit level 7 write-up**<br>

##*Objective*:<br>The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size<br>

##Steps taken:<br>

*1.Connecting to sever* <br>

Used the SSH command to login to the server with the copied password<br>
Command: ssh bandit6@bandit.labs.overthewire.org -p 2220<br>

*2.find the file which has the password* <br>

Command: find / -type f -user bandit7 -group bandit6 -size 33c<br>

*3.Get the Password *<br>
Command: cat /var/lib/dpkg/info/bandit7.password <br>
copy the text as it is the password for the next level

*4.Close the Connection*<br>
Command: exit
