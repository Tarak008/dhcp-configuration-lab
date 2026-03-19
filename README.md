# 🔧 DHCP Configuration Lab

## 📌 Objective
To configure DHCP server to automatically assign IP addresses to clients in a network.

---

## 🖥️ Network Topology
- 1 Router
- 1 Switch
- 1 Server (DHCP)
- 2 PCs

---

## 🌐 IP Addressing Scheme

| Device | IP Address | Subnet Mask | Gateway |
|--------|-----------|-------------|--------|
| Router | 192.168.1.1 | 255.255.255.0 | - |
| Server | 192.168.1.2 | 255.255.255.0 | 192.168.1.1 |

---

## ⚙️ Configuration Steps

### Router Configuration
```bash
enable
configure terminal
interface fa0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
```

### DHCP Server Configuration
- Pool Name: DHCP_POOL
- Default Gateway: 192.168.1.1
- DNS: 8.8.8.8
- Start IP: 192.168.1.10

---

## 🧪 Testing
- Set PC to DHCP
- Use `ipconfig` to verify IP assignment

---

## 📸 Screenshots
See screenshots folder.
---

## ✅ Result
Successfully assigned IP addresses dynamically using DHCP.

---

## 🔐 Skills Gained
- DHCP Configuration
- Network Troubleshooting
- IP Address Management
