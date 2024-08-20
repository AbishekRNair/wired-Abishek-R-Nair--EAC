#**Bandit level 2 write-up**<br>

##*Objective*:<br>The password for the next level is stored in a file called - located in the home directory.<br>

##Steps taken:<br>

*1.Connecting to sever* <br>

Used the SSH command to login to the server with the provided password<br>
Command: ssh bandit1@bandit.labs.overthewire.org -p 2220<br>

*2.Get the Password for the next level from - directory*<br>
Command: cat ./- <br>
copy the text as it is the password for the next level

*3.Close the Connection*<br>
Command: exit
