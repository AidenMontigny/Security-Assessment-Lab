<h1> Security Assessment Lab </h1>

<h2>Description</h2>
This project demonstrates the practical execution of a network security assessment using tools such as Nmap and OpenVAS (GVM). The assessment begins with network scanning to identify active hosts and their associated IP addresses, followed by in-depth service and OS fingerprinting. After identifying targets, OpenVAS is used to perform vulnerability scans, allowing for the discovery and documentation of potential security issues. The process includes configuring scan targets, executing scans, and reviewing results in terms of CVEs and known vulnerabilities. This assignment reinforces core concepts of vulnerability management, secure network configuration, and structured assessment workflows. It concludes with detailed recommendations to mitigate discovered vulnerabilities, emphasizing patch management, access control, network segmentation, multi-factor authentication, and continuous monitoring.
<br />

<h2>Languages and Utilities Used</h2>

- <b> Command Line </b>  
- <b>OpenVAS (Greenbone Vulnerability Manager)</b>  
- <b>Linux Shell (Bash)</b>  
- <b>CVSS/CVE Analysis Tools</b>  

<h2>Environments Used </h2>

- <b> Kali Linux Virtual Machine </b>

<h2>Project walk-through:</h2>

<p align="left">
The process began with launching Nmap on the virtual machine to conduct a network scan, <br/> identifying active hosts and their open ports. <br/><br/>
  <img src="Screenshot 2025-05-01 120856.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
After identifying the hosts and their corresponding IP addresses, a more comprehensive scan <br/>  was conducted to fingerprint the operating systems and enumerate active services. <br/><br/>
  <img src="Screenshot 2025-05-01 120903.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
The scan results provided insight into the network topology and exposed services, enabling <br/> targeted vulnerability assessments in subsequent steps. <br/><br/>
  <img src="Screenshot 2025-05-01 120912.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
The Greenbone Security Assistant shows an active vulnerability scan nearing completion. <br/><br/>
  <img src="Screenshot 2025-05-01 120923.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
Greenbone Security Assistant provides an overview of vulnerabilities identified during the <br/> scan, categorizing them by severity, detailing their specific characteristics such as  <br/> detection dates, severity scores, and affected hosts, while also offering filtering and sorting options based on scan quality. <br/><br/>
  <img src="Screenshot 2025-05-01 120930.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
Greenbone Security Assistant displays an overview of detected CVEs, including severity <br/> classifications, creation trends, CVSS scores, and detailed vulnerability information. <br/><br/>
  <img src="Screenshot 2025-05-01 120937.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
Repeat steps 1-7 for the remaining two targets, starting with identifying their IP <br/>  addresses, which in this case are 192.168.0.1 and 192.168.0.2. <br/><br/>
  <img src="Screenshot 2025-05-01 120949.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
The image displays a table titled "Targets 3 of 3" with three targets and their respective <br/>  IP addresses. <br/><br/>
  <img src="Screenshot 2025-05-01 120957.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
The dashboard provides an overview of 183,963 CVEs, categorized by severity. It includes <br/>  visualizations of CVE trends over time and a table listing specific vulnerabilities with  <br/> descriptions, published dates, and CVSS base scores. <br/><br/>
  <img src="Screenshot 2025-05-01 121005.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
This list displays vulnerabilities detected by Greenbone Security Assistant, including <br/>  issues like "Microsoft SMB Signing Disabled" and "ICMP Timestamp Detection."  <br/><br/>
  <img src="Screenshot 2025-05-01 121018.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>


<h2>Write Up</h2>

<p><u> Recommendations </u></p>
<p>To comprehensively address and eliminate identified vulnerabilities, a multi-faceted security strategy must be established. A foundational layer involves the regular application of security patches, including monthly cycles for operating systems and applications. As well, network segmentation should be implemented to isolate critical systems, thereby minimizing the potential impact of a breach. Enforcing the principle of least privilege for user accounts, demonstrated through frequent reviews and adjustments of user roles and permissions, effectively reduces the attack surface and mitigates the risk of unauthorized access. The integration of multi-factor authentication, especially within login processes for sensitive applications, adds a layer of security. Continuous monitoring facilitated by intrusion detection systems and log analysis tools allows for real-time threat detection and swift responses to security incidents. The development and regular updating of an incident response plan and routine security awareness training for employees enhance the organization's agility in responding to security events and diminish the risk of human error. Augmenting these measures, implementing encryption for sensitive data in transit and at rest, conducting regular penetration testing and security audits, maintaining comprehensive documentation of security measures, and yearly reviews and updates to security policies contribute significantly to a resilient security posture. This holistic approach, tailored to the organization's needs, establishes a robust framework for mitigating vulnerabilities and advancing overall cybersecurity.
</p>
