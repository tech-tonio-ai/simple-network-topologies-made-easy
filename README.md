# 🌐 Simple Network Topologies Made Easy  

![Network Topology Overview](path/to/topology-screenshot.png)  

## 📌 About This Repository  
This repository is a **beginner-friendly** guide to understanding basic network topologies using **Layer 2 switches, Layer 3 switches, wireless routers, and end devices**. Each section contains a **diagram**, a **brief explanation**, and relevant **switch/router configurations**.  

---

## 🖥️ Network Topology Overview  
🔹 **Devices Used:**  
- 1x Layer 2 Switch  
- 1x Layer 3 Switch  
- 1x Wireless Router  
- 2-3 Computers  

🔹 **Purpose:**  
- Demonstrate basic network setups  
- Show fundamental switch & router configurations  
- Provide practical CLI examples  

---

## 🏗️ Network Setup & Configuration  

### **1️⃣ VLAN Configuration on L2 Switch**  
📷 _Screenshot of VLAN configuration_  
![VLAN Configuration](path/to/vlan-screenshot.png)  

```bash
# Create VLANs
enable
configure terminal
vlan 10
name SALES
vlan 20
name IT
exit

```
```bash
# Enable Inter-VLAN Routing
enable
configure terminal
interface vlan 10
ip address 192.168.10.1 255.255.255.0
interface vlan 20
ip address 192.168.20.1 255.255.255.0
exit
