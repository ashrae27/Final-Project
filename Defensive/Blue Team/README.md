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
- Purpose: Apache
- IP Address: 192.168.1.110/24

### Target 2
- Operation System: Debian/Linux 8
- Purpose: Apache
- IP Address: 192.168.1.115/24

### Elk
- Operation System: Ubuntu 18.0.4
- Purpose: Host Machine
- IP Address: 19.168.1.100

### Capstone
- Operation System: Ubuntu 18.04.1 LTS
- Purpose: Victim machine
- IP Address: 192.168.1.105

### Description of Targets
TODO: Answer the questions below.
The target of this attack was: Target 1 (TODO: IP Address).
Target 1 is an Apache web server and has SSH enabled, so ports 80 and 22 are possible ports of entry for attackers. As such, the following alerts have been implemented:

Monitoring the Targets
Traffic to these services should be carefully monitored. To this end, we have implemented the alerts below:

## Name of Alert 1
TODO: Replace Alert 1 with the name of the alert.
Alert 1 is implemented as follows:

- Metric: TODO
- Threshold: TODO
- Vulnerability Mitigated: TODO

Reliability: TODO: Does this alert generate lots of false positives/false negatives? Rate as low, medium, or high reliability.

## Name of Alert 2
Alert 2 is implemented as follows:

- Metric: TODO
- Threshold: TODO
- Vulnerability Mitigated: TODO

Reliability: TODO: Does this alert generate lots of false positives/false negatives? Rate as low, medium, or high reliability.

## Name of Alert 3
Alert 3 is implemented as follows:

- Metric: TODO
- Threshold: TODO
- Vulnerability Mitigated: TODO

Reliability: TODO: Does this alert generate lots of false positives/false negatives? Rate as low, medium, or high reliability.

TODO Note: Explain at least 3 alerts. Add more if time allows.

### Suggestions for Going Further (Optional)
TODO:

- Each alert above pertains to a specific vulnerability/exploit. Recall that alerts only detect malicious behavior, but do not stop it. For each vulnerability/exploit identified by the alerts above, suggest a patch. E.g., implementing a blocklist is an effective tactic against brute-force attacks. It is not necessary to explain how to implement each patch.

The logs and alerts generated during the assessment suggest that this network is susceptible to several active threats, identified by the alerts above. In addition to watching for occurrences of such threats, the network should be hardened against them. The Blue Team suggests that IT implement the fixes below to protect the network:

### Vulnerability 1
- Patch: TODO: E.g., install special-security-package with apt-get
- Why It Works:

Why It Works: TODO: E.g., special-security-package scans the system for viruses every day

### Vulnerability 2
- Patch: TODO: E.g., install special-security-package with apt-get
- Why It Works: TODO: E.g., special-security-package scans the system for viruses every day

### Vulnerability 3
 - Patch: TODO: E.g., install special-security-package with apt-get
 - Why It Works: TODO: E.g., special-security-package scans the system for viruses every da
