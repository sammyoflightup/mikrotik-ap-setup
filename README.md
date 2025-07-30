[Quick Command Cheat Shee.txt](https://github.com/user-attachments/files/21514663/Quick.Command.Cheat.Shee.txt)[Quick Command Cheat Shee.txt](https://github.com/user-attachments/files/21514644/Quick.Command.Cheat.Shee.txt)# mikrotik-ap-setup
Step-by-step guide to setting up MikroTik routers as access points for seamless WiFi across a space. Includes diagrams, config tips, and cheat sheets.
# MikroTik Access Point Setup Guide

This project helps beginners configure multiple MikroTik routers into a single, secure, and seamless WiFi network across a home, office, or studio.

## Goal
Create a stable WiFi system where:
- One main router handles internet + DHCP
- Other MikroTik devices act as Access Points (APs)
- All devices share the same SSID (WiFi name)
- Seamless handoff between devices (no need to switch networks)

---

## What’s Inside
- Setup Cheat Sheet (Printable)
-  Draw.io Network Diagram
-  RouterOS CLI commands
-  Step-by-step breakdown (human language)

---

## 🛠 Basic Steps

1. **Reset all routers**
2. **Configure the Main Router:**
   - Set internet access
   - Enable DHCP
3. **Configure Each Access Point (AP):**
   - Assign static IP
   - Disable DHCP Server
   - Bridge ports
   - Match WiFi name and password
4. **Connect all APs via LAN cables to main router**

---

## 📎 Files

![Diagram](https://github.com/user-attachments/assets/e0d7c7f2-6125-4408-9acc-fa6658d90366)
[How to Set Up a Single Secure WiFi Network.pdf](https://github.com/user-attachments/files/21514662/How.to.Set.Up.a.Single.Secure.WiFi.Network.pdf)

[Uploading Q/ip address add address=192.168.88.2/24 interface=ether1
/ip dhcp-client remove 0
/ip dhcp-server disable 0
/interface wireless set [find] ssid="YourWiFi" disabled=no
/interface bridge add name=bridge1
/interface bridge port add interface=ether1 bridge=bridge1
/interface bridge port add interface=wlan1 bridge=bridge1
uick Command Cheat Shee.txt…]()



---

## Contributing
Feel free to fork and adjust for your own layout or use case. Contributions welcome.

---
