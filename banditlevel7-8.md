#**Bandit level 8 write-up**<br>

##*Objective*:<br>The password for the next level is stored in the file data.txt next to the word millionth<br>

##Steps taken:<br>

*1.Connecting to sever* <br>

Used the SSH command to login to the server with the copied password<br>
Command: ssh bandit7@bandit.labs.overthewire.org -p 2220<br>

*2.find the password* <br>

Command: cat data.txt<br>
Command: strings data.txt | grep "millionth"<br>

*3.Get the Password*<br>
copy the text as it is the password for the next level

*4.Close the Connection*<br>
Command: exit
