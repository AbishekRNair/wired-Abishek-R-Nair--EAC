#Bandit level 14-15 write-up

##Objective:The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level.
##Steps taken: 1.Connecting to server

Used the SSH command to login to the server with the provided password

Command: ssh bandit14@bandit.labs.overthewire.org -p 2220

2.Connecting to localhost at port 30000

Using nc command connected to the localhost at port 30000 after entering the password found the password for next level
Command:nc localhost 30000
