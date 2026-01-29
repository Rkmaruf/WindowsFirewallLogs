# Windows Firewall Logs Analysis and Rule Configuration

## 📌 Project Overview

This project focuses on analyzing **Windows Defender Firewall logs** to monitor, understand, and detect suspicious or malicious network activity. It also demonstrates how to create, configure, and verify inbound and outbound firewall rules to enhance system security.

The project is designed for **cybersecurity learning, network monitoring, and defensive security practices**.

---

## ⚠️ Disclaimer

This project is intended for **educational and research purposes only**.  
All experiments were performed in a controlled environment.  
Unauthorized network monitoring or rule manipulation may violate laws and policies.

---

## 🎯 Project Objectives

- Monitor network traffic using Windows Firewall logs
- Analyze dropped and allowed packets
- Detect suspicious or malicious activities
- Verify firewall rule effectiveness
- Understand inbound and outbound traffic control
- Improve Windows system security

---

## 🛠️ Tools and Environment

- Windows Operating System
- Windows Defender Firewall
- Notepad / Text Editor
- Administrator Access

---

## 📖 Why Firewall Logging Is Important

Firewall logging helps to:

- Verify newly added firewall rules
- Debug misconfigured rules
- Detect blocked or dropped packets
- Identify application connectivity issues
- Monitor outgoing suspicious connections
- Detect possible attack attempts
- Improve incident response

Examples of suspicious activity:
- Unexpected outbound connections
- Repeated dropped packets
- Unauthorized port access
- Malicious scanning attempts

---

## 🧪 Step 1: Enable Windows Firewall Logging

### Procedure

1. Open **Windows Defender Firewall**.
2. Click **Properties**.
3. Select **Domain Profile** → **Logging** → **Customize**.
4. Enable logging options (set to **Yes**).
5. Click **OK**.
6. Repeat the same process for:
   - Private Profile
   - Public Profile
7. Verify all logging settings.

---

## 🧪 Step 2: Access Firewall Log Files

### Method

1. Go to **Monitoring** → **Logging Settings**.
2. Click the file path to open logs.
3. View log activities.

### Default Log Location
C:\Windows\System32\LogFiles\Firewall\pfirewall.log



Logs can be opened using Notepad or any text editor.

---

## 🧪 Step 3: Create Inbound Firewall Rules

### Objective
Control incoming traffic to the system.

### Procedure

1. Open **Inbound Rules**.
2. Click **New Rule**.
3. Select **Port**.
4. Choose **TCP** and specify ports.
5. Select **Block the connection**.
6. Choose desired profiles (Domain/Private/Public).
7. Assign a rule name.
8. Finish setup.

### Result
Inbound rules are successfully configured.

---

## 🧪 Step 4: Create Outbound Firewall Rules

### Objective
Control outgoing network traffic.

### Procedure

Outbound rules follow the same steps as inbound rules.

1. Open **Outbound Rules**.
2. Create new rules using port or custom options.
3. Configure block/allow policies.
4. Save the rules.

### Result
Outbound traffic filtering is enabled.

---

## 🧪 Step 5: Block Websites Using Firewall Rules

### Objective
Prevent access to specific websites or domains.

### Procedure

1. Click **New Rule** → Select **Custom**.
2. Choose **All Programs**.
3. Proceed to **Scope**.
4. Add target website IP addresses.
   - IPv4
   - IPv6
5. Select **Block the connection**.
6. Choose profiles.
7. Assign a rule name.
8. Finish.


### Result
Target website is successfully blocked.

---

## 🧪 Step 6: Block Incoming Ping (ICMP)

### Objective
Prevent ICMP echo requests (ping) to enhance security.

### Procedure

1. Create a new inbound rule.
2. Select **Custom**.
3. Choose **All Programs**.
4. Select **ICMPv4/ICMPv6**.
5. Choose **Block the connection**.
6. Select profiles.
7. Name the rule.
8. Finish.

### Result
Incoming ping requests are blocked.

---

## 🧪 Step 7: Extract Firewall Logs

### Procedure

1. Open the log file path.
2. View logs in Notepad.
3. Save logs for analysis.


---

## 🧪 Step 8: Analyze Firewall Logs

### Objective
Verify rule performance and detect blocked activities.

### Analysis Process

- Open `pfirewall.log`
- Search for:
  - DROP entries
  - Blocked IPs
  - Blocked ports
  - Blocked domains
- Match log entries with created rules

### Example Findings

- Blocked website requests
- Dropped packets
- Denied connections
- Rule enforcement confirmation

---

## 📊 Observations

- Firewall logs provide valuable network insights
- Rules effectively block unwanted traffic
- Unusual outbound traffic can indicate compromise
- Log analysis improves threat detection
- Proper configuration enhances system security

---

## ✅ Conclusion

This project demonstrates how Windows Defender Firewall logging and rule configuration can be used to:

- Monitor network activity
- Detect suspicious behavior
- Control inbound and outbound connections
- Improve system defense
- Validate security policies

Firewall log analysis is an essential skill for cybersecurity professionals.

---

## 🚀 Future Improvements

- Automate log analysis using scripts
- Integrate SIEM tools
- Apply advanced filtering
- Implement alert systems
- Perform real-time monitoring
- Study attack pattern detection

---

## 👤 Author

**Name:** Ruhul kinbria Maruf  
**Project Type:** Cyber Security / Network Defense  
**Purpose:** Academic & Practical Learning

---

## 📅 Date

Aprill 4th 2024

---

Thank you.


