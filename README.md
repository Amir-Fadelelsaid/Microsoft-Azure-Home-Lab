Azure-Defense-Lab

📌 Project Overview

Azure-Defense-Lab is a cybersecurity home lab designed to simulate real-world SOC (Security Operations Center) analyst tasks. It leverages Azure, Windows, Microsoft Sentinel, and Defender for Endpoint to detect and respond to malware, providing hands-on experience in threat monitoring and incident response.

🫠 Tools & Technologies Used

Azure Virtual Machines – Windows instance for endpoint monitoring

Microsoft Sentinel – Cloud-native SIEM and SOAR solution

Microsoft Defender for Endpoint – Endpoint Detection & Response (EDR) solution

Windows Event Logs – Log collection for security analysis

PowerShell – Agent installation and configuration

🚀 Features

Deploys a Windows virtual machine in Azure

Installs Microsoft Defender for Endpoint for endpoint monitoring

Configures Microsoft Sentinel to collect and analyze logs

Simulates malware detection using the EICAR test file

Responds to threats just like a SOC analyst

🏰 Setup Instructions

1️⃣ Deploy Windows Instance in Azure

Create an Azure account (Azure Free Tier).

Navigate to the Azure Portal and create a Windows Virtual Machine.

Configure networking to allow RDP access (port 3389).

Create and download an RDP key pair to access your instance.

Connect to the instance using Remote Desktop Protocol (RDP).

2️⃣ Set Up Microsoft Sentinel

Navigate to the Azure Portal and search for Microsoft Sentinel.

Deploy a Log Analytics Workspace and onboard it to Sentinel.

Enable security analytics and configure log ingestion.

3️⃣ Install & Configure Defender for Endpoint Agent

In Microsoft Defender Security Center, navigate to "Onboarding".

Generate an installation script for Windows.

Run the script in PowerShell on the Azure VM.

Verify that logs are being ingested in Microsoft Sentinel.

4️⃣ Simulate Malware Detection

Download the EICAR test file.

Attempt to execute it on the Windows VM.

Microsoft Defender for Endpoint should detect and quarantine the file.

Review the alert in Microsoft Sentinel under the Incidents tab.

📊 Use Cases & Learning Outcomes

✅ Understand SIEM architecture and log ingestion✅ Gain hands-on experience in malware detection & response✅ Learn to configure endpoint security agents✅ Practice SOC analyst workflows with alert analysis & triage

🎯 Future Enhancements

🫠 Automate deployment using Terraform

🔍 Expand to Linux/macOS agents for cross-platform monitoring

📊 Create custom detection rules in Microsoft Sentinel

🔒 Integrate Splunk or other SIEM tools for comparative analysis

🏆 Acknowledgments

Built as a hands-on cybersecurity project to simulate real-world SOC workflows and gain practical experience in threat detection & incident response. Inspired by Microsoft Security Best Practices and Azure security principles.
