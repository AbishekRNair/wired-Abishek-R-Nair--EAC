#**Bandit level 5 write-up**<br>

##*Objective*:<br>The password for the next level is stored in a file called - located in the home directory.<br>

##Steps taken:<br>

*1.Connecting to sever* <br>

Used the SSH command to login to the server with the copied password<br>
Command: ssh bandit4@bandit.labs.overthewire.org -p 2220<br>

*2.Change directory to inhere and find the human readable file* <br>

Command: cd inhere<br>
Command: find . -type f | xargs file<br>

*3.Get the Password for the next level from hidden file*<br>
Command: cat ./-file07 <br>
copy the text as it is the password for the next level

*4.Close the Connection*<br>
Command: exit
