# Wireshark-Network-Analysis-Lab
Objective:** Capture, filter, and analyze different types of network traffic (DNS, ICMP, HTTPS, QUIC) to demonstrate baseline traffic monitoring and anomaly detection skills.
# 🦈 Wireshark Network Analysis Lab  
**Objective:** Capture, filter, and analyze different types of network traffic (DNS, ICMP, HTTPS, QUIC) to demonstrate baseline traffic monitoring and anomaly detection skills.  

---

## 🔧 Setup
- **Tool:** Wireshark (with Npcap driver installed)  
- **System:** Windows 11 Desktop  
- **Interfaces:** Wi-Fi & Ethernet (captured on both for comparison)  

---

## 📡 Captures

### 1. DNS Lookups  
Filter:  
```dns```  

- Captured DNS queries and responses while browsing the web.  
- ✅ Confirms the ability to isolate name resolution traffic.  

📸 Screenshot:  
![DNS Traffic](images/dns-filter.png)

---

### 2. ICMP Ping Test  
Filter:  
```icmp```  

- Sent ping requests to Google’s DNS server (`8.8.8.8`).  
- ✅ Shows echo request/reply workflow.  

📸 Screenshot:  
![ICMP Ping](images/ping.png)

---

### 3. ICMP Ping Flood (Noisy Traffic Simulation)  
Command used:  
```bash
ping 8.8.8.8 -t
