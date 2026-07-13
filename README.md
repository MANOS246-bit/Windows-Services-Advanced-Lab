# Windows_Services_Advanced_Lab
# Windows 10 Services Advanced Lab

## 🛡️ Στόχος

Δημιουργία ενός εργαστηρίου σε **Windows 10** για εξάσκηση στη διαχείριση των Windows Services, στον έλεγχο της κατάστασης υπηρεσιών μέσω GUI και Command Prompt, στη διαχείριση του Windows Firewall και στη βασική αντιμετώπιση προβλημάτων δικτύου.

Πραγματοποιήθηκαν δοκιμές σε:

* Windows Services
* Service Status Verification
* Service Identification using CLI
* Windows Firewall
* ICMP Firewall Rules
* VirtualBox Networking (NAT → Bridged)

Σκοπός: πρακτική εξάσκηση σε **Windows Administration, Troubleshooting, Networking και IT Support skills**.

---

## 🖥️ Περιβάλλον

* OS: Windows 10 Pro
* Tools:
  * Services (services.msc)
  * Command Prompt (Administrator)
  * Windows Firewall with Advanced Security
  * VirtualBox
  * Windows Update

---

## 🔧 Lab Activities

### Windows Update Service

Verified the Windows Update service using both the graphical interface and the command line.

**Screenshots**

* [Windows Update Properties](./Windows_Service_Status/1_wuauserv_properties.png)
* [Service State Before](./Windows_Service_Status/2_wuauserv_state_before.png)
* [Service State After](./Windows_Service_Status/3_wuauserv_state_after.png)

**Commands**

```cmd
sc query wuauserv
```

**Result**

* Verified the Windows Update service status.
* Confirmed that the service starts automatically after selecting **Check for updates**.

---

### Service Identification

Located a Windows service using Command Prompt and verified it through Services.

**Screenshots**

* [Service Properties](./Service_Identification/1_service_properties.png)
* [SC Query Spooler](./Service_Identification/2_sc_query_spooler.png)

**Command**

```cmd
sc query spooler
```

**Result**

* Identified a Windows service using the command line.
* Verified the same service in the Services management console.
* Demonstrated how CLI can help locate services that are not immediately visible in the GUI.

---

### Windows Firewall

Verified the active Windows Firewall profile and configured an inbound ICMP blocking rule.

**Screenshots**

* [Current Firewall Profile](./Windows_Firewall/1_current_firewall_profile_cmd.png)
* [Inbound ICMP Rule](./Windows_Firewall/2_inbound_rule_block_icmp_public.png)
* [Ping Block Test](./Windows_Firewall/3_ping_block_test.png)

**Commands**

```cmd
wf.msc

netsh advfirewall show currentprofile
```

**Result**

* Verified the active firewall profile.
* Created an inbound ICMP blocking rule.
* Confirmed that ping requests were successfully blocked.

---

### VirtualBox Networking

Changed the VirtualBox network adapter from NAT to Bridged mode and verified network connectivity.

**Screenshots**

* [Bridged Adapter](./Windows_Firewall/4_virtualbox_bridged_mode.png)
* [Successful Ping](./Windows_Firewall/5_ping_success_bridged.png)

**Result**

* Changed the network adapter from NAT to Bridged.
* Successfully restored communication between virtual machines.

---

### Advanced Windows Services

Explored additional Windows Service configuration options.

**Screenshots**

* [Service Status](./Windows_Services_Advanced/1_service_status.png)
* [Recovery Settings](./Windows_Services_Advanced/2_recovery_settings.png)
* [Dependencies](./Windows_Services_Advanced/3_dependencies.png)
* [Troubleshooting Error](./Windows_Services_Advanced/4_troubleshooting_error.png)

**Result**

* Examined service status.
* Reviewed recovery options.
* Inspected service dependencies.
* Observed troubleshooting information for service errors.

---

## 🧠 Τι Έμαθα

* Verify Windows service status using GUI and CLI.
* Use **sc query** to inspect Windows services.
* Identify Windows services through Command Prompt.
* Configure and verify Windows Firewall rules.
* Test ICMP traffic blocking.
* Understand VirtualBox NAT and Bridged networking.
* Analyze Windows service recovery options and dependencies.
* Improve Windows administration and troubleshooting skills.

---

## 🛠️ Tools

| Tool | Purpose |
|------|---------|
| Windows 10 Pro | Lab environment |
| Services (services.msc) | Windows service management |
| Command Prompt | Service management using CLI |
| sc | Query Windows services |
| Windows Firewall | Firewall configuration |
| netsh advfirewall | Firewall profile management |
| VirtualBox | Network virtualization |

---

## 💼 CV Entry

Managed Windows Services using both GUI and Command Prompt, verified Windows Update service behavior, configured Windows Firewall ICMP rules, analyzed service recovery settings and dependencies, and tested VirtualBox NAT and Bridged networking to strengthen Windows administration, troubleshooting and IT support skills.

---

## 👤 About me

📍 Computer Systems Technician specializing in **Windows Administration, Networking, Linux and IT Support**

📫 LinkedIn / Email

[LinkedIn Profile](https://www.linkedin.com/in/%CE%B5%CE%BC%CE%BC%CE%B1%CE%BD%CE%BF%CF%85%CE%B7%CE%BB-%CE%BA%CE%B1%CE%BD%CE%B1%CE%BA%CE%B7%CF%82-695809356/)

[kanakismanolis04@gmail.com](mailto:kanakismanolis04@gmail.com)
