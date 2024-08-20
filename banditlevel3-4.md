#**Bandit level 4 write-up**<br>

##*Objective*:<br>The password for the next level is stored in a file called - located in the home directory.<br>

##Steps taken:<br>

*1.Connecting to sever* <br>

Used the SSH command to login to the server with the copied password<br>
Command: ssh bandit3@bandit.labs.overthewire.org -p 2220<br>

*2.Change directory to inhere and find the hidden file* <br>

Command: cd inhere<br>
Command: ls -alph<br>

*3.Get the Password for the next level from hidden file*<br>
Command: cat ...hidden-from-you <br>
copy the text as it is the password for the next level

*4.Close the Connection*<br>
Command: exit
