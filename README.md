# Network Security Audit – DRDO Subcontractor Environment

## 📌 Objective
Perform a basic internal network audit covering device configuration, access control, firewall rule review, segmentation, and vulnerability observation.

## 🏢 Environment
- Routers & switches (Cisco & HP mix)
- 20+ LAN endpoints
- Controlled DRDO-linked secure workflow
- Firewall with ACL-based policies  

> *Direct access to mission-critical systems was restricted. Work included observation, documentation, and reviewing allowed components.*

---

## 🔍 Audit Components

### **1. Router & Switch Configuration Review**
- Verified VLAN assignments  
- Checked routing tables  
- Identified unused interfaces  
- Confirmed SNMP & telnet/SSH access securely configured  

### **2. Access-Control Review**
- Mapped ACL rules  
- Identified overly broad allow rules  
- Observed improper segmentation between user VLANs  

### **3. Firewall Rule Assessment**
- Validated inbound/outbound rules  
- Checked NAT & zone policies  
- Documented rule gaps (e.g., ANY-ANY rules)  

### **4. Device Inventory & Cabling**
- Documented device list: switches, routers, APs  
- Confirmed cable labeling & physical security  

---

## 🛠 Issues Identified

### **Issue 1: Broad ACL rules**
- Some VLANs had wide access  
- Missing least-privilege rule design  

### **Issue 2: No centralized change log**
- Firewall & ACL changes were not logged consistently  

### **Issue 3: Weak segmentation**
- Sensitive workstation group had lateral communication exposure  

---

## 🩹 Recommendations

### **1. Implement least privilege**
Restrict VLAN-to-VLAN communication.

### **2. Enable rule change logging**
Maintain a structured firewall change document.

### **3. Introduce network segmentation**
Separate sensitive systems from general user traffic.

---

## 🎯 Key Learnings
- Gained audit-style exposure to real network environments  
- Understood secure communication flows  
- Collaborated with senior engineers for configuration review  
