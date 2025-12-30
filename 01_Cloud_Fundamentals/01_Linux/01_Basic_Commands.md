🐧 Linux Fundamentals – Simple & Practical Notes

Linux is an open-source operating system used in almost all cloud servers (AWS, Azure, Snowflake, etc.).
It allows us to control servers, manage files, install software and automate tasks using commands and shell scripts.


📍 Navigation & System Commands

pwd     = Show current location  
ls      = Show files & folders  
ls -l   = Detailed list  
ls -a   = Show hidden files  
cd dir  = Go inside folder  
cd ..   = Go back  
clear   = Clear terminal  
whoami  = Current user  
uname -a= OS details  
history = Show command history  
date    = Show date & time  
exit    = Exit terminal  


📁 File & Folder Management

mkdir test      = Create folder  
rmdir test      = Delete empty folder  
rm -r test      = Delete folder with data  
touch file.txt  = Create file  
cp a b          = Copy file  
mv a b          = Rename / Move  
cat file.txt    = View file  
less file.txt   = Scroll view  
head file.txt   = First lines  
tail file.txt   = Last lines  
find / -name x  = Find file  


🔐 Permissions

r = Read  
w = Write  
x = Execute  

chmod 777 file  = Full permission  
chmod 755 file  = Owner full access  
chown user file = Change file owner  
ls -l           = View permissions  


📦 Package Management

sudo apt update         = Refresh packages  
sudo apt install nginx = Install software  
sudo apt remove nginx  = Remove software  


🌐 Networking

ip a             = Show IP  
ping google.com  = Check internet  
netstat -tulnp   = Open ports  
curl google.com  = Test website  


🧠 Process Management

ps        = Running processes  
top       = Live CPU/RAM view  
kill PID  = Stop process  


🧾 Shell Scripting Basics

#!/bin/bash          = Script start  
echo "Hello"        = Print text  
read name           = Take input  
if [ $a -gt $b ]    = If condition  
for i in 1 2 3      = Loop  
while true          = Infinite loop  
sh file.sh          = Run script  
./file.sh           = Execute script  


