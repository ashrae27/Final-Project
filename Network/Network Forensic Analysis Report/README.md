# Network Forensic Analysis Report

### Time Thieves
You must inspect your traffic capture to answer the following questions:

What is the domain name of the users' custom site?

**frank -in -ted.com** 

What is the IP address of the Domain Controller (DC) of the AD network?

**10.6.12.0/24**

What is the name of the malware downloaded to the 10.6.12.203 machine?

**GET/files/june.dll HTTP**

Once you have found the file, export it to your Kali machine's desktop.
 
![Activity Day 3 malware](https://user-images.githubusercontent.com/88813019/157806113-eaac2324-3cc6-46c2-97d4-f273ac069c61.PNG)

What kind of malware is this classified as?
 
**Trojan spy/mint**

### Vulnerable Windows Machine

1. Find the following information about the infected Windows machine:

- Host name **Rottendam-PC**
- IP address **172.16.4.205*
- MAC address **00:59:07:60:63**

2. What is the username of the Windows user whose computer is infected?

**matthijs devries**

3. What are the IP addresses used in the actual infection traffic?

![Screenshot 2022-03-09 210207](https://user-images.githubusercontent.com/88813019/157806448-d0827c42-0111-4de0-923d-a76ff188d621.png)

### Illegal Downloads
1. Find the following information about the machine with IP address 10.0.0.201:

- MAC address **00:16:17:18:66:C8*
- Windows username **SNamestring**
- OS version **Windows NT 10:0**
 2. Which torrent file did the user download?

**type=torrent and file=Betty_Book_Rythm_the_Reservatiion.avi.torrent HTTP/.1.1 /r /n**
