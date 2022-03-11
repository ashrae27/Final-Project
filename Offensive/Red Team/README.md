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

- Target 1

List of Exposed Services:
- Port 22 (SSH)
- Port 80 (HTTP)
- Port 111 (rcpbind)

The following vulnerabilities were identified on each target:

- Target 1
- List of
- Critical
- Vulnerabilities

TODO: Include vulnerability scan results to prove the identified vulnerabilities.

## Exposed Services

The following vulnerabilities were identified on each target:

Target 1
- Identification and Authentication Failures
- Weak passwords
- Unprotected files
- User Enumeration (WordPress)

TODO: Include vulnerability scan results to prove the identified vulnerabilities.

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
