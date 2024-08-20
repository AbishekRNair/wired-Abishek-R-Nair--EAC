#**Bandit level 10 write-up**<br>

##*Objective*:<br>The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.<br>

##Steps taken:<br>

*1.Connecting to sever* <br>

Used the SSH command to login to the server with the copied password<br>
Command: ssh bandit9@bandit.labs.overthewire.org -p 2220<br>

*2.find the password* <br>

Command: strings data.txt | grep "="<br>

*3.Get the Password*<br>
copy the text as it is the password for the next level

*4.Close the Connection*<br>
Command: exit
