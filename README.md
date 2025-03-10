# Azure-Defense-Lab

## 📌 Project Overview
Azure-Defense-Lab is a **cybersecurity home lab** designed to simulate real-world **SOC (Security Operations Center) analyst** tasks. It leverages **Azure, Windows, Microsoft Sentinel, and Log Analytics Workspace** to detect and respond to live attacks, providing hands-on experience in threat monitoring and incident response.

## 🛠 Tools & Technologies Used
- **Azure Virtual Machines** – Cloud-based honeypot for monitoring attacks
- **Microsoft Sentinel** – Cloud-native SIEM for security event management
- **Log Analytics Workspace** – Centralized log repository for event analysis
- **Windows Event Logs** – Log collection for security monitoring
- **PowerShell** – Agent installation and configuration

## 🚀 Features
- Deploys a **Windows virtual machine** in Azure as a honeypot
- Configures **Microsoft Sentinel** to collect and analyze logs
- Simulates **real-world attacks** by exposing the VM to the internet
- Extracts **geolocation data** to map attackers in real time
- Responds to threats **just like a SOC analyst**

## 🏗️ Setup Instructions

### **1️⃣ Deploy Windows Virtual Machine in Azure**
1. Create an **[Azure Free Account](https://azure.microsoft.com/en-us/free/)**.
2. Launch a **Windows Virtual Machine** using a free-tier eligible size.
3. Configure **Remote Desktop Protocol (RDP)** for access.
4. Set up **Network Security Group (NSG)** to allow all inbound traffic.
5. Disable **Windows Firewall** inside the VM.

### **2️⃣ Configure Log Analytics Workspace**
1. Create a **Log Analytics Workspace** in the same Resource Group.
2. Connect the **Virtual Machine** to **Log Analytics**.
3. Install the **Azure Monitoring Agent** on the VM to forward logs.

### **3️⃣ Set Up Microsoft Sentinel**
1. Activate **Microsoft Sentinel** and connect it to Log Analytics Workspace.
2. Install **Windows Security Event Connector** to collect logs.
3. Enable **Security Event Collection** for ingestion.

### **4️⃣ Simulate Malware Attacks**
1. Leave the VM exposed to the public internet.
2. Attackers will attempt **brute-force logins** within minutes.
3. View **failed login attempts** in Event Viewer inside the VM.
4. Use **Sentinel Queries (KQL)** to analyze attack patterns.

### **5️⃣ Enrich Logs with Geolocation Data**
1. Upload an **IP Geolocation Database** to Sentinel as a **Watchlist**.
2. Match attacker IP addresses to **cities and countries**.
3. Use **KQL queries** to extract attacker locations.

### **6️⃣ Create an Attack Map in Sentinel**
1. Open **Sentinel Workbooks** and create a new dashboard.
2. Import a **KQL Query** to visualize attack sources on a world map.
3. Track live attack data and adjust map settings as needed.

## 📊 Use Cases & Learning Outcomes
✅ Understand **SIEM architecture** and log ingestion  
✅ Gain hands-on experience in **threat intelligence & analysis**  
✅ Learn **KQL querying** for attack investigations  
✅ Build an **interactive attack map** in Microsoft Sentinel  
✅ Practice **SOC analyst workflows** with **real attack data**

## 🔮 Future Enhancements
- 🛠 **Automate deployment** using Terraform & Azure Bicep
- 🔍 **Expand to Linux/macOS agents** for broader coverage
- 📈 **Enhance detection rules** for advanced threat analysis
- 🔒 **Integrate with Splunk & other SIEM tools** for cross-platform monitoring

## 🏆 Acknowledgments
Built as a hands-on cybersecurity project to simulate **real-world SOC workflows** and gain **practical experience** in threat detection & incident response. Inspired by **Microsoft Sentinel Labs** and best practices in cloud security.
