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
