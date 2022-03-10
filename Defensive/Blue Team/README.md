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

- Metric: TODO
- Threshold: TODO
- Vulnerability Mitigated: TODO

Reliability: TODO: Does this alert generate lots of false positives/false negatives? Rate as low, medium, or high reliability.

## HTTP Request Size Monitor
Alert 2 is implemented as follows:

- Metric: TODO
- Threshold: TODO
- Vulnerability Mitigated: TODO

Reliability: TODO: Does this alert generate lots of false positives/false negatives? Rate as low, medium, or high reliability.

## CPU Usage Monitor
Alert 3 is implemented as follows:

- Metric: TODO
- Threshold: TODO
- Vulnerability Mitigated: TODO

Reliability: TODO: Does this alert generate lots of false positives/false negatives? Rate as low, medium, or high reliability.

TODO Note: Explain at least 3 alerts. Add more if time allows.

The logs and alerts generated during the assessment suggest that this network is susceptible to several active threats, identified by the alerts above. In addition to watching for occurrences of such threats, the network should be hardened against them. The Blue Team suggests that IT implement the fixes below to protect the network:

### Vulnerability 1
- Patch: TODO: E.g., install special-security-package with apt-get
- Why It Works:

### Vulnerability 2
- Patch: TODO: E.g., install special-security-package with apt-get
- Why It Works: TODO: E.g., special-security-package scans the system for viruses every day

### Vulnerability 3
 - Patch: TODO: E.g., install special-security-package with apt-get
 - Why It Works: TODO: E.g., special-security-package scans the system for viruses every da
