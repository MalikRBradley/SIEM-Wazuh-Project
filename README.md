# 🔍 Windows Security Detection Lab with Wazuh + Sysmon (Azure SOC Simulation)

This hands-on project demonstrates how to detect suspicious activity on a Windows 11 VM using **Wazuh** (deployed on Azure) and **Sysmon** for detailed endpoint telemetry. The simulation involves creating a fake admin account and launching a brute-force attack to trigger alerts and visualize real-time detection.

---

## 🛠️ Tools & Environment

- **Wazuh SIEM** (v4.11.2, deployed on Ubuntu VM via Azure)
- **Sysmon** for Windows Event ID telemetry
- **Windows 11 VM** for adversary simulation
- **Kali Linux** (Hydra brute-force testing)
- **Microsoft Azure** (NSG configuration, VM management)
- **Parallels/VMware** on Mac M3 ARM64

---

## 🚨 What Was Simulated

- Created a fake admin account on Windows using PowerShell
- Installed and configured Sysmon agent
- Captured Windows Event ID changes in Wazuh
- Launched a brute-force RDP attack using Hydra from Kali
- Validated alerts in Wazuh's Threat Hunting and Event dashboards

---

## 📸 Screenshots

### Wazuh Login Page
![Image](<img width="1728" alt="Screenshot 2025-05-05 at 2 46 57 PM" src="https://github.com/user-attachments/assets/f9ff469e-ff1b-4980-8000-5cf556be3620" />)

### Active Sysmon Agent (Windows 11 VM)
![Wazuh Agent Active](./Screenshot%202025-05-05%20at%202.49.27%20PM.jpeg)

### Azure NSG Rules for Exposure Simulation
![Azure NSG](./Screenshot%202025-05-06%20at%201.01.44%20PM.jpeg)

### Event ID 4625 (Failed Logon Attempt)
![Event 4625](./Screenshot%202025-05-06%20at%208.35.02%20AM.jpeg)

### Brute-Force Attempt from Kali (Hydra)
![Hydra Attempt](./Screenshot%202025-05-06%20at%206.51.01%20AM.jpeg)

### Threat Hunting in Wazuh Dashboard
![Threat Hunting](./Screenshot%202025-05-06%20at%208.29.54%20AM.jpeg)

### Windows Event Viewer Capturing Activity via Sysmon
![Sysmon Event Viewer](./Screenshot%202025-05-06%20at%208.27.13%20AM.jpeg)

---

## ✅ Skills Demonstrated

- Cloud-based SIEM deployment
- Endpoint detection & response (EDR) using Sysmon
- Event correlation and alert analysis
- Network Security Group (NSG) configuration
- Brute-force attack simulation and detection
- Real-time event monitoring & log analysis

---

## 💡 Lessons Learned

- How to map Windows Event IDs to malicious behavior
- Importance of telemetry from agents like Sysmon
- Wazuh’s capability to visualize and respond to incidents
- Best practices for isolating and monitoring exposed endpoints

---

## 👤 Author

**Malik R. Bradley**  
Cybersecurity Enthusiast | Blue Team Projects  
[LinkedIn](https://www.linkedin.com/in/malik-bradley-a1273b28a/) • [GitHub](https://github.com/MalikRBradley)

---

> ⚠️ *This lab was created in a safe, isolated Azure environment for educational use only.*
