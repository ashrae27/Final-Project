# Blue Team: Summary of Operations

## Table of Contents

- Network Topology
- Description of Targets
- Monitoring the Targets
- Patterns of Traffic & Behavior
- Suggestions for Going Further
### Network Topology
The following machines were identified on the network:

![Target Server Diagram](https://user-images.githubusercontent.com/88813019/157139657-0a211372-34ac-459a-8236-5a21e8c2702d.png)

### Kali Linux
- Operating System: Linux (Debian)
- Purpose: Pen testing machine
- IP Address: 192.168.1.90

### Target 1
- Operating System: Debian/Linux 8
- Purpose: Vulnerability WordPress Attack 2
- IP Address: 192.168.1.110/24

### Elk
- Operation System: Ubuntu 18.0.4
- Purpose: Access to Web to view alerts
- IP Address: 19.168.1.100

### Capstone
- Operation System: Ubuntu 18.04.1 LTS
- Purpose: Alert testing Attack target
- IP Address: 192.168.1.105

### Description of Targets.
The target of this attack was: 

#### Target 1
![activity day 2  part 1 Target 1 IP Address](https://user-images.githubusercontent.com/88813019/157151854-efcd21a9-ff4b-4a45-a72c-0af818498936.PNG)

Target 1 open ports are:
- SSH (22)
- HTTP (80) 
- rpcbind(111).

Monitoring the Targets
Traffic to these services should be carefully monitored. To this end, we have implemented the alerts below:

## Excessive HTTP Errors
Alert 1 is implemented as follows:

- Metric: WHEN count () GROUPED OVER top 5 'http. response.status_code' IS ABOVE 400 FOR THE LAST 5 minutes
- Threshold: IS ABOVE 400
- Vulnerability Mitigated: Brute Force Attacks

Reliability: The alert will let the SOC team know if there are any alerts above 400 that allow the team to analyze the server errors. If there are multiple errors in a short time, it could become a brute force attack.

## HTTP Request Size Monitor
Alert 2 is implemented as follows:

- Metric: WHEN sum () OF http.request.bytes OVER all documents IS ABOVE 3500 FOR THE LAST 1 minute
- Threshold: 3500
- Vulnerability Mitigated: Cross site script of Denial of Service attacks

Reliability: The alert will let us know there are a large number of HTTP requests and some requests have not hurt our systems.

## CPU Usage Monitor
Alert 3 is implemented as follows:

- Metric: WHEN max () OF system.process.cpu.total.pct OVER all documents IS ABOVE 0.5 FOR THE LAST 5 minutes
- Threshold: IS ABOVE0.5 
- Vulnerability Mitigated: Malicious programs take up to 0.5% CPU usage

Reliability: The alert can identify issues in CPU performance and make it a system upkeep.

The logs and alerts generated during the assessment suggest that this network is susceptible to several active threats, identified by the alerts above. In addition to watching for occurrences of such threats, the network should be hardened against them. The Blue Team suggests that IT implement the fixes below to protect the network:

### Excessive HTTP Errors
- Patch: Hardening wordpress and wordpress implement

- Why It Works: Updates to wordpress and easy implement fixes exploits/vulnerabilites

It can provide implements such as:
- Firewall
- Ifconfig
Wordpress can include users
- Vuew all the users and helpts mitiagte in case of enumeration attacks

### HTTP Request Size Monitor
- Patch: Injection and DDoS
 Execution of HTTP
Boundries on the webservers can include 
- highest URL length
- Highest size

- Why It Works: 404 errors will happen due to HTTP appeal URl length and the size limit of the request. Data validation helps protect against malicious data from attackers who attempt to send the server through the website or across an HTTP appeal.


### CPU Usage Monitor
 - Patch: TODO: E.g., install special-security-package with apt-get
 - Why It Works: TODO: E.g., special-security-package scans the system for viruses every da
