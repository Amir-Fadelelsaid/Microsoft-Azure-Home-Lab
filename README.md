Azure-Defense-Lab

📌 Project Overview

Azure-Defense-Lab is a cybersecurity home lab designed to simulate real-world SOC (Security Operations Center) analyst tasks. It leverages Azure, Windows, Microsoft Sentinel, and Log Analytics Workspace to detect and respond to live attacks, providing hands-on experience in threat monitoring and incident response.

🧰 Tools & Technologies Used

Azure Virtual Machines – Cloud-based honeypot for monitoring attacks

Microsoft Sentinel – Cloud-native SIEM for security event management

Log Analytics Workspace – Centralized log repository for event analysis

Windows Event Logs – Log collection for security monitoring

PowerShell – Agent installation and configuration

🚀 Features

Deploys a Windows virtual machine in Azure as a honeypot

Configures Microsoft Sentinel to collect and analyze logs

Simulates real-world attacks by exposing the VM to the internet

Extracts geolocation data to map attackers in real time

Responds to threats just like a SOC analyst

🏰 Setup Instructions

1️⃣ Create an Azure Subscription

Sign up for an Azure Free Account.

Provide a credit card for verification (no charges during the trial).

Log in to portal.azure.com.

2️⃣ Deploy Windows Virtual Machine

Create a Resource Group (e.g., RG-SOC-Lab).

Create a Virtual Network and Subnet inside the Resource Group.

Deploy a Windows 10 Virtual Machine:

Use a free-tier eligible VM size.

Set up Remote Desktop Protocol (RDP) access.

Configure a Network Security Group (NSG):

Open all inbound traffic to attract attackers.

Disable Windows Firewall to allow unrestricted access.

3️⃣ Configure Log Analytics Workspace

Create a Log Analytics Workspace in the same Resource Group.

Connect the Virtual Machine to Log Analytics.

Install the Azure Monitoring Agent on the VM to forward logs.

4️⃣ Set Up Microsoft Sentinel

Activate Microsoft Sentinel and connect it to Log Analytics Workspace.

Install Windows Security Event Connector to collect VM logs.

Enable Security Event Collection for log ingestion.

5️⃣ Simulate Live Attacks

Leave the VM exposed to the public internet.

Attackers will attempt to brute-force logins within minutes to hours.

Log into the VM and view failed login attempts using Event Viewer.

Configure Sentinel Queries (KQL) to analyze failed login patterns.

6️⃣ Enrich Logs with Geolocation Data

Upload an IP Geolocation Database to Sentinel as a Watchlist.

Match attacker IP addresses to cities and countries.

Use KQL queries to extract attacker locations.

7️⃣ Create an Attack Map

Open Sentinel Workbooks and create a new dashboard.

Import a preconfigured KQL Query to visualize attacks on a world map.

Track live attack data and adjust map settings for better insights.

📊 Use Cases & Learning Outcomes

✅ Understand SIEM architecture and log ingestion✅ Gain hands-on experience in threat intelligence & analysis✅ Learn KQL querying for attack investigations✅ Build an interactive attack map in Microsoft Sentinel✅ Practice SOC analyst workflows with real attack data

🌟 Future Enhancements

🛠 Automate deployment using Terraform & Azure Bicep

🔎 Expand to Linux/macOS agents for broader coverage

📊 Enhance detection rules for advanced threat analysis

🔒 Integrate with Splunk & other SIEM tools for cross-platform monitoring

🏆 Acknowledgments

Built as a hands-on cybersecurity project to simulate real-world SOC workflows and gain practical experience in threat detection & incident response. Inspired by Microsoft Sentinel Labs and best practices in cloud security.

