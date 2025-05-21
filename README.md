# 🔍 Windows Security Detection Lab with Wazuh + Sysmon (Azure SOC Simulation)

This hands-on project demonstrates how to detect suspicious activity on a Windows 11 VM using **Wazuh** (deployed on Azure) and **Sysmon** for detailed endpoint telemetry. The simulation involves creating a fake admin account and launching a brute-force attack to trigger alerts and visualize real-time detection.

---

## 🛠️ Tools & Environment

- **Wazuh SIEM** (v4.11.2, deployed on Ubuntu VM via Azure)
- **Sysmon** for Windows Event ID telemetry
- **Windows 11 VM** for adversary simulation
- **Kali Linux** (Hydra brute-force testing)
- **Microsoft Azure** (NSG configuration, VM management)
- **VMware** on Mac M3 ARM64

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
![Image](https://github.com/user-attachments/assets/f9ff469e-ff1b-4980-8000-5cf556be3620)

### Active Sysmon Agent (Windows 11 VM)
![Image](https://github.com/user-attachments/assets/8c78a3d4-c38f-487f-8f56-7b0b204f64df)

### Azure NSG Rules for Exposure Simulation
![Image](https://github.com/user-attachments/assets/a2c8ba23-a8a5-461a-9ca6-47498f2f106d)

### Event ID 4625 (Failed Logon Attempt)
![Image](https://github.com/user-attachments/assets/46a800c4-3564-4061-921c-d80c8fc441f3)

### Brute-Force Attempt from Kali (Hydra)
![Image](https://github.com/user-attachments/assets/2fcc8c60-e585-4490-b229-ecb0f3a62e67)
hydra -t 4 -v -f -l windowsuser -P /usr/share/wordlists/rockyou.txt rdp://20.127.233.1
### Threat Hunting in Wazuh Dashboard
![Image](https://github.com/user-attachments/assets/503215b5-6020-4c83-bbf6-bc6052bfaccd)

### Windows Event Viewer Capturing Activity via Sysmon
![Image](https://github.com/user-attachments/assets/faca3fbc-1e2a-4105-b50a-5ad9c8e7a2ee)

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
