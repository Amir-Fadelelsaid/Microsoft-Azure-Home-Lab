<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Microsoft Azure Home Lab</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #121212;
            color: #fff;
        }
        .container {
            max-width: 900px;
            margin: auto;
            padding: 20px;
            background: #1e1e1e;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 150, 255, 0.2);
        }
        h1, h2, h3 {
            color: #00a8ff;
        }
        a {
            color: #00a8ff;
            text-decoration: none;
            font-weight: bold;
        }
        a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Microsoft Azure Home Lab</h1>
        
        <h2>📌 Project Overview</h2>
        <p>Microsoft-Azure-Home-Lab is a cloud-based cybersecurity lab designed to simulate SOC (Security Operations Center) operations. Using Microsoft Sentinel, Azure Virtual Machines (VMs), and KQL queries, this lab enables real-time threat detection by analyzing live attacks on an intentionally exposed VM.</p>
        
        <h2>🛠 Tools & Technologies Used</h2>
        <ul>
            <li>Microsoft Sentinel – Cloud-native SIEM for security event monitoring</li>
            <li>Azure Virtual Machines (Windows 10) – Honeypot for collecting attack data</li>
            <li>Azure Log Analytics Workspace – Centralized security log repository</li>
            <li>Network Security Group (NSG) – Cloud firewall with intentional open access</li>
            <li>Kusto Query Language (KQL) – Querying security logs for threat analysis</li>
            <li>GeoIP Data Mapping – Visualizing attack origins on a world map</li>
        </ul>
        
        <h2>🚀 Features</h2>
        <ul>
            <li>Deploys a Windows VM as a public-facing honeypot to attract real-world attacks</li>
            <li>Uses Azure Monitoring Agent to collect failed login attempts (Event ID 4625)</li>
            <li>Sends logs to Log Analytics Workspace for centralized security event analysis</li>
            <li>Queries attack data using KQL to detect brute-force attempts</li>
            <li>Visualizes attacker locations in Microsoft Sentinel’s Windows VM Attack Map Workbook</li>
        </ul>
        
        <h2>🏗️ Setup Instructions</h2>
        <h3>1️⃣ Deploy a Windows VM in Azure</h3>
        <ol>
            <li>Sign up for an <a href="https://azure.microsoft.com/en-us/free/" target="_blank">Azure Free Subscription</a>.</li>
            <li>Create a Resource Group and Virtual Network.</li>
            <li>Deploy a Windows 10 Virtual Machine in East US 2 region.</li>
            <li>Assign a Public IP and configure the Network Security Group (NSG).</li>
            <li>Disable Windows Firewall to allow external access.</li>
        </ol>
        
        <h3>2️⃣ Connect VM Logs to Microsoft Sentinel</h3>
        <ol>
            <li>Create an Azure Log Analytics Workspace.</li>
            <li>Install the Azure Monitoring Agent on the VM.</li>
            <li>Configure log forwarding to Microsoft Sentinel.</li>
        </ol>
        
        <h3>3️⃣ Simulate Real-World Attacks</h3>
        <ol>
            <li>Expose the VM to the internet and wait for brute-force login attempts.</li>
            <li>Query failed login attempts (Event ID 4625) in Sentinel using KQL.</li>
            <li>Identify attacker IP addresses and attack patterns.</li>
        </ol>
        
        <h3>4️⃣ Visualize Attacks with the Windows VM Attack Map</h3>
        <ol>
            <li>Download the Windows VM Attack Map Workbook JSON file.</li>
            <li>Import it into Microsoft Sentinel &gt; Workbooks.</li>
            <li>Observe real-time GeoIP attack data plotted on a world map.</li>
        </ol>
        
        <h2>📊 Use Cases & Learning Outcomes</h2>
        <ul>
            <li>Gain hands-on experience in SIEM security monitoring</li>
            <li>Understand Azure Virtual Machines & cloud security configurations</li>
            <li>Learn KQL (Kusto Query Language) for log analysis</li>
            <li>Practice incident response & threat detection using real attack data</li>
            <li>Build SOC analyst skills by monitoring and investigating live security events</li>
        </ul>
        
        <h2>🔮 Future Enhancements</h2>
        <ul>
            <li>🛠 Automate deployment using Terraform for scalable SOC labs</li>
            <li>🔍 Integrate other SIEM tools (Splunk, Wazuh, Elastic) for comparative analysis</li>
            <li>📊 Enhance detection rules in Sentinel for advanced threat correlation</li>
            <li>🔒 Experiment with Azure Security Center & Defender for Cloud</li>
        </ul>
        
        <h2>🏆 Acknowledgments</h2>
        <p>Built to simulate real-world SOC workflows, this project enhances security operations and incident response skills using Microsoft Sentinel & Azure.</p>
        
        <h3>📂 GitHub Repository: <a href="#">Microsoft-Azure-Home-Lab</a></h3>
        <h3>📺 YouTube Demo: <a href="#">Watch the Full Video</a></h3>
    </div>
</body>
</html>
