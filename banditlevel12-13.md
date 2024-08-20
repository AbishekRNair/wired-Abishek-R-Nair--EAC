#Bandit level 12-13 write-up

##Objective:The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv

Used the SSH command to login to the server with the provided password

Command: ssh bandit12@bandit.labs.overthewire.org -p 2220

2.Finding the file

Using ls command found the file data.txt

Command:ls

3.Creating temp directory

Using mktemp command created temp directory

Command:mktemp -d

4.Copying data.txt to temp file

Using cp command copied data.txt to temp file

Command:cp /home/bandit12/data.txt /tmp/tmp.UmYCjx1hWx

5.Changed name and extension

Using mv command renamed the file

Command:mv data.txt compressedfile.hex

6.Converted the hexdump back into its original binary format

Using xxd command converted the hexdump back into its original binary format

Command:xxd -r compressedfile.hex compressedfile.bin

7.Analysing the file type and extracting the file

Using file and extracting commands repeatedly to get the ASCII text file

Commands:file compressedfile.bin
mv compresssedfile.bin compressedfile.gz
gunzip compressedfile.gz
bunzip2 data6.bz2
tar -xf data8.bin

8.Opening the file and getting the password

Using cat command opened the final ouput file after extraction to get password

Command:cat data8
