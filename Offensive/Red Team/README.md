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


## Exploitation

The Red Team was able to penetrate Target 1 and retrieve the following confidential data:

Target 1


flag1.txt: TODO: Insert flag1.txt hash value


Exploit Used

TODO: Identify the exploit used
TODO: Include the command run

flag2.txt: TODO: Insert flag2.txt hash value


Exploit Used

TODO: Identify the exploit used
TODO: Include the command run
