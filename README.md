Microsoft Azure Home Lab
📌 Project Overview
Microsoft-Azure-Home-Lab is a cloud-based cybersecurity lab designed to simulate SOC (Security Operations Center) operations. Using Microsoft Sentinel, Azure Virtual Machines (VMs), and KQL queries, this lab enables real-time threat detection by analyzing live attacks on an intentionally exposed VM.

🛠 Tools & Technologies Used
Microsoft Sentinel – Cloud-native SIEM for security event monitoring
Azure Virtual Machines (Windows 10) – Honeypot for collecting attack data
Azure Log Analytics Workspace – Centralized security log repository
Network Security Group (NSG) – Cloud firewall with intentional open access
Kusto Query Language (KQL) – Querying security logs for threat analysis
GeoIP Data Mapping – Visualizing attack origins on a world map
🚀 Features
Deploys a Windows VM as a public-facing honeypot to attract real-world attacks
Uses Azure Monitoring Agent to collect failed login attempts (Event ID 4625)
Sends logs to Log Analytics Workspace for centralized security event analysis
Queries attack data using KQL to detect brute-force attempts
Visualizes attacker locations in Microsoft Sentinel’s Windows VM Attack Map Workbook
🏗️ Setup Instructions
1️⃣ Deploy a Windows VM in Azure
Sign up for an Azure Free Subscription.
Create a Resource Group and Virtual Network.
Deploy a Windows 10 Virtual Machine in East US 2 region.
Assign a Public IP and configure the Network Security Group (NSG).
Disable Windows Firewall to allow external access.
📸 Azure Virtual Machine Setup: View Screenshot

2️⃣ Connect VM Logs to Microsoft Sentinel
Create an Azure Log Analytics Workspace.
Install the Azure Monitoring Agent on the VM.
Configure log forwarding to Microsoft Sentinel.
📸 Azure Log Analytics Workspace: View Screenshot

3️⃣ Simulate Real-World Attacks
Expose the VM to the internet and wait for brute-force login attempts.
Query failed login attempts (Event ID 4625) in Sentinel using KQL.
Identify attacker IP addresses and attack patterns.
📸 Failed Logins in Sentinel (KQL Query Results): View Screenshot

4️⃣ Visualize Attacks with the Windows VM Attack Map
Download the Windows VM Attack Map Workbook JSON file.
Import it into Microsoft Sentinel > Workbooks.
Observe real-time GeoIP attack data plotted on a world map.
📸 Windows VM Attack Map Workbook in Sentinel: View Screenshot

📊 Use Cases & Learning Outcomes
✅ Gain hands-on experience in SIEM security monitoring
✅ Understand Azure Virtual Machines & cloud security configurations
✅ Learn KQL (Kusto Query Language) for log analysis
✅ Practice incident response & threat detection using real attack data
✅ Build SOC analyst skills by monitoring and investigating live security events

🔮 Future Enhancements
🛠 Automate deployment using Terraform for scalable SOC labs
🔍 Integrate other SIEM tools (Splunk, Wazuh, Elastic) for comparative analysis
📊 Enhance detection rules in Sentinel for advanced threat correlation
🔒 Experiment with Azure Security Center & Defender for Cloud
🏆 Acknowledgments
Built to simulate real-world SOC workflows, this project enhances security operations and incident response skills using Microsoft Sentinel & Azure.

📂 GitHub Repository: Microsoft-Azure-Home-Lab
📺 YouTube Demo: Watch the Full Video
