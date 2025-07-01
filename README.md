<p align="center">
  <a href="https://github.com/Samuel-Cavada" target="_blank">
    <img src="https://img.shields.io/badge/Back_to_Main_Page-000000?style=for-the-badge&logo=github&logoColor=white" alt="Back to Main Page"/>
  </a>
</p>

<h1 align="center">Onboarding a VM to Microsoft Defender for Endpoint (MDE): VM Isolation and Investigation </h1>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" alt="Cloud Platform" />
  <img src="https://img.shields.io/badge/OS-Windows%2010-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="OS" />
  <img src="https://img.shields.io/badge/Tool-Microsoft%20Defender%20for%20Endpoint-00B388?style=for-the-badge&logo=microsoftdefender&logoColor=white" alt="Tool" />
  <img src="https://img.shields.io/badge/Tool-PowerShell-2C5EA8?style=for-the-badge&logo=powershell&logoColor=white" alt="Tool" />
  <img src="https://img.shields.io/badge/Focus-Endpoint%20Security-orange?style=for-the-badge" alt="Focus Area" />
</p>

---

## 📌 Project Objective
> Successfully onboard a Windows 10 virtual machine to Microsoft Defender for Endpoint (MDE), practice isolating the device from the network, and collect an investigation package for endpoint forensics.

---

## 🧰 Tools & Technologies
- **Platform:** Azure
- **OS:** Windows 10
- **Tools:** Microsoft Defender for Endpoint, Azure VM, PowerShell
- **Languages/Scripts:** Windows GUI, CLI

---

## 🧠 Skills Gained / Focus Areas
- Onboarded a VM to MDE and verified success
- Isolated a device using the MDE portal
- Collected and inspected forensic investigation packages
- Practiced proactive security measures and incident response

---

## 🧪 Environment Setup
> Provisioned a secure Windows 10 VM in Azure. Downloaded and installed the MDE onboarding package using administrator privileges. Configured network and firewall rules to support testing and isolation behavior.

![Onboarding a VM to MDE - Image 0](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%200.jpg?raw=true)

---

## 🛠️ Walkthrough
1. [Step 1: Onboard the VM](#step-1-onboard-the-vm)
2. [Step 2: Isolate the VM](#step-2-isolate-the-vm)
3. [Step 3: Collect an Investigation Package](#step-3-collect-an-investigation-package)

---

### ✅ Step 1: Onboard the VM
> - Created a Windows 10 VM in Azure with secure credentials  
> - Logged into the [Microsoft Defender portal](https://security.microsoft.com)  
> - Navigated to: **Settings → Endpoints → Device Management → Onboarding**  
> - Downloaded the Windows 10/11 MDE onboarding package (provided by admin)  
> - Installed the package inside the VM (Right-click → Run as Administrator)  
> - Verified onboarding success at **Assets → Devices**

![Onboarding a VM to MDE - Image 1](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%201.jpg?raw=true)
![Onboarding a VM to MDE - Image 2](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%202.jpg?raw=true)
![Onboarding a VM to MDE - Image 3](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%203.jpg?raw=true)
![Onboarding a VM to MDE - Image 4](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%204.jpg?raw=true)


---

### ✅ Step 2: Isolate the VM
> - Turned off Windows Firewall (`wf.msc`)  
> - Modified NSG to allow inbound ICMP  
> - Started a ping loop from an external device to the VM’s public IP  
> - Logged into MDE Portal → **Assets → Devices**  
> - Selected the VM → Clicked 3-dot menu → Chose “Isolate Device”  
> - Observed the ping drop due to isolation  
> - Later: released the device from isolation for continued use

![Onboarding a VM to MDE - Image 10](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%210.jpg?raw=true)

![Onboarding a VM to MDE - Image 5](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%205.jpg?raw=true)

![Onboarding a VM to MDE - Image 6](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%206.jpg?raw=true)

![Onboarding a VM to MDE - Image 7](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%207.jpg?raw=true)

![Onboarding a VM to MDE - Image 8](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%208.jpg?raw=true)

![Onboarding a VM to MDE - Image 9](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%209.jpg?raw=true)


---

### ✅ Step 3: Collect an Investigation Package
> - In MDE Portal: **Assets → Devices**  
> - Selected device → Clicked 3-dot menu → “Collect Investigation Package”  
> - Entered a comment and confirmed  
> - Viewed progress in the **Action Center**  
> - Once completed, downloaded the package  
> - Unzipped and inspected artifacts such as logs, memory, registry, and binaries

![Onboarding a VM to MDE - Image 11](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%2011.jpg?raw=true)

![Onboarding a VM to MDE - Image 12](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%2012.jpg?raw=true)

![Onboarding a VM to MDE - Image 13](https://github.com/Samuel-Cavada/Onboarding-a-VM-to-MDE/blob/main/images/Onboarding-a-VM-to-MDE%2013.jpg?raw=true)


---

## 📝 Outcomes and Lessons Learned
- **Technical Insight:** Onboarding enables visibility into detailed endpoint activity and supports rapid investigation.
- **Configuration Skills:** Managed onboarding, isolation, and package collection from the Defender portal.
- **Troubleshooting:** Verified device connectivity, firewall settings, and package success using the MDE dashboard.
- **Takeaway:** Device onboarding is a foundational step for endpoint protection and incident response in modern enterprise environments.

---

## 📎 References
- [Microsoft Defender for Endpoint Portal](https://security.microsoft.com)
- [MDE Onboarding Documentation](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/configure-endpoints-mdc)
- [MDE Investigation Package Details](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/investigation-packages)
