# Security-Automation
Security Automation (Python / Bash)

<h2>Introduction</h2>
This project demonstrates a practical implementation of Security Operations Center (SOC) automation using Python and Bash scripting. The goal is to simulate a simplified real world SOC workflow by automating the process of log analysis, threat intelligence enrichment, and alert triage.

Modern SOC environments generate large volumes of log data, making manual analysis inefficient and error-prone. To address this challenge, this project builds a lightweight automation pipeline that:

* Parses system or web server logs to identify suspicious activity
* Extracts potential Indicators of Compromise (IOCs), such as IP addresses
* Enriches these indicators using the VirusTotal API
* Automatically assigns severity levels based on threat intelligence results

By combining log parsing, API integration, and decision making logic, this project reflects core tasks performed by SOC analysts and highlights the growing importance of automation in cybersecurity operations.
<br />


<h2>Tools & Environment Used</h2>

- <b>OS: Debian 13.x (VM on MacBook)</b> 
- <b>Virtualization: VMware Fusion</b>
- <b>Language: Python</b>
- <b>Scripting: Bash</b>
- <b>API: VirusTotal</b>
- <b>Libraries: requests, re, time</b>

<h2>Project Snapshots:</h2>

<p align="center">
I started this project by updating the Linux OS: <br/>
<img src="https://i.postimg.cc/0yJ7Dcfy/1-Update-OS.png" height="80%" width="80%" alt="OS Update"/>
<br />
<br />
I created new files & folder for this project: <br/>
<img src="https://i.postimg.cc/76bs2jKC/2-Create-files-and-folder.png" height="80%" width="80%" alt="New Folder"/>
<br />
<br />
At the time of this project I did not use real data source so I created fake logs:
<br />
<br/>
<img src="https://i.postimg.cc/CKbLV6GW/3-fake-logs.png" height="80%" width="80%" alt="Fake Logs"/>
<br />
<br />
I created log parser using python script:  <br/>
<img src="https://i.postimg.cc/VsZw2cx2/4-python-script.png" height="80%" width="80%" alt="Log Parser"/>
<br />
<br />
I verified the python script is working:  <br/>
<img src="https://i.postimg.cc/zBXmPd0F/5-result.png" height="80%" width="80%" alt="Python Script"/>
<br />
<br />
Setting up Threat Enrichment, I signed up with virus total and I copied the API Key:  <br/>
<img src="https://i.postimg.cc/rs0Pv7Wp/6-api-key.png" height="80%" width="80%" alt="API Key"/>
<br />
<br />
Enrichment scripts using python:  <br/>
<img src="https://i.postimg.cc/6pyFR2Td/7-vt-python-script.png" height="80%" width="80%" alt="Enrichment"/>
<br />
<br />
Confirmed enrichment script result:  <br/>
<img src="https://i.postimg.cc/fTsPHqLq/8-enrichment-list.png" height="80%" width="80%" alt="Enrichment"/>
<br />
<br />
Built an auto triage script:  <br/>
<img src="https://i.postimg.cc/qRwdQfrB/9-Triage-script.png" height="80%" width="80%" alt="Automation"/>
<br />
<br />
Confirmed Auto-triage script:  <br/>
<img src="https://i.postimg.cc/k5CZHjfx/10-run-triage-script.png" height="80%" width="80%" alt="Automation"/>
<br />
<br />
I Automated the scripts using bash command:  <br/>
<img src="https://i.postimg.cc/8z0tVZpm/11-Bash-Script.png" height="80%" width="80%" alt="Automation"/>
<br />
<br />
Verifying that Automation is working:  <br/>
<img src="https://i.postimg.cc/wM4ssbb1/12-Automation.png" height="80%" width="80%" alt="Verify Automation"/>
<br />
</p>


<h2>Skills Demonstrated </h2>

- <b>Security automation</b>
- <b>Log analysis</b>
- <b>Threat intelligence integration</b>
- <b>Python scripting</b>
- <b>Bash scripting</b>
- <b>SOC workflow understanding</b>

<h2>Summary </h2>
<p>
In this project, a complete end-to-end security automation workflow was successfully developed. The system begins by analyzing log files to detect suspicious patterns, such as unauthorized access attempts or probing behaviour. Identified IP addresses are then enriched using external threat intelligence data, allowing the system to assess whether they are associated with malicious activity.

Based on the enrichment results, an automated triage process classifies each event into severity levels (e.g., Low, Medium, High), enabling faster prioritization and response. The entire pipeline can be executed manually or through a single Bash script, demonstrating how repetitive SOC tasks can be streamlined efficiently.

This project showcases foundational cybersecurity skills, including log analysis, scripting, API usage, and alert prioritization. It also provides a scalable base for future enhancements such as real-time monitoring, integration with SIEM platforms, and automated alerting systems. Overall, it reflects the practical application of automation to improve efficiency and effectiveness in modern SOC environments.

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
