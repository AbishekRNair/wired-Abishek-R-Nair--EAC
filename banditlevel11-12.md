#**Bandit level 12 write-up**<br>

##*Objective*:<br>The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions<br>

##Steps taken:<br>

*1.Connecting to sever* <br>

Used the SSH command to login to the server with the copied password<br>
Command: ssh bandit11@bandit.labs.overthewire.org -p 2220<br>

*2.find the password* <br>

Command: cat data.txt<br>
copy the text and past it in https://gchq.github.io/CyberChef/ to get the password


*3.Get the Password*<br>
copy the text as it is the password for the next level

*4.Close the Connection*<br>
Command: exit
