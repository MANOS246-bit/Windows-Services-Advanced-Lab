# Windows 10 Services & Firewall Administration Lab

## 🛡️ Στόχος

Δημιουργία ενός εργαστηρίου σε **Windows 10** για εξάσκηση στη διαχείριση των Windows Services, στην επαλήθευση της κατάστασης υπηρεσιών μέσω GUI και Command Prompt, στη διαμόρφωση του Windows Firewall και στη βασική αντιμετώπιση προβλημάτων δικτύου.

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

Verified the Windows Update service status using both the graphical interface and Command Prompt.

**Screenshots**

* [Windows Update Properties](./screenshots/Windows-Update-Properties.png)
* [Service State Before](./screenshots/Service-State-Before.png)
* [Service State After](./screenshots/Service-State-After.png)

**Command**

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

* [Service Properties](./screenshots/service-properties.png)
* [SC Query Spooler](./screenshots/sc-query-spooler.png)

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

* [Current Firewall Profile/Inbound ICMP Rule](./screenshots/netsh-advfirewall-show-currentprofile.png)
* [Ping Block Test](./screenshots/ping-command.png)

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

* [Bridged Adapter](./screenshots/virtualbox-bridged-mode.png)
* [Successful Ping](./screenshots/Succesful-Ping.png)

**Result**

* Changed the network adapter from NAT to Bridged.
* Successfully restored network communication between the host and virtual machine.

---

### Advanced Windows Services

Explored additional Windows Service configuration options in "Guide to creating inbound connection rules".

**Screenshots**

* [Rule](./screenshots/Type-of-Rule.png)
* [Program](./screenshots/Program.png)
* [Protocol](./screenshots/Protocol-and-Ports.png)
* [Range](./screenshots/width-range.png)
* [Actions](./screenshots/Action.png)
* [Profile](./screenshots/Profile.png)

**Result**

* Verified Windows service status.
* Reviewed Recovery options.
* Analyzed service dependencies.
* Examined service error reporting and troubleshooting information.
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
* Verify Windows Firewall profiles using netsh.
* Understand Windows service startup behavior.

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

Managed Windows Services using both GUI and Command Prompt, verified Windows Update behavior, configured Windows Firewall ICMP rules, analyzed service recovery settings and dependencies, and configured VirtualBox networking (NAT and Bridged) to strengthen Windows administration, troubleshooting and networking skills.

---

## 👤 About me

📍 Computer Systems Technician specializing in **Windows Administration, Networking, Linux and IT Support**

📫 LinkedIn / Email

[LinkedIn Profile](https://www.linkedin.com/in/%CE%B5%CE%BC%CE%BC%CE%B1%CE%BD%CE%BF%CF%85%CE%B7%CE%BB-%CE%BA%CE%B1%CE%BD%CE%B1%CE%BA%CE%B7%CF%82-695809356/)

[kanakismanolis04@gmail.com](mailto:kanakismanolis04@gmail.com)
