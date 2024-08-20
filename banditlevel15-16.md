#Bandit level 15-16 write-up

##Objective: The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.

Used the SSH command to login to the server with the provided password

Command: ssh bandit15@bandit.labs.overthewire.org -p 2220

2.Connecting to localhost at port 30001

Using openssl command connected to the localhost at port 30001 with the provided password found the password for next level

Command:openssl s_client -connect localhost:30001
