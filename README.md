# Ubuntu-server-secure2

sudo nft -f /etc/nftables.conf
sudo nft list ruleset

sudo systemctl enable nftables
sudo systemctl start nftables

sudo cp /etc/nftables.conf /etc/nftables.conf.bak

sudo nano /etc/nftables.conf
sudo nft -f /etc/nftables.conf


# 🛡️ Ubuntu 24.04 Security Hardening Guide
## Tools Covered:
- ✅ SELinux (via `selinux-basics`)
- ✅ AppArmor
- ✅ Firewalld

---

## 🔐 1. SELinux (Optional for Ubuntu)

Ubuntu does **not** ship with SELinux enabled by default — it uses AppArmor instead. But if you want to experiment with it:

### 🧰 Install SELinux Support
```bash
sudo apt update
sudo apt install selinux-basics selinux-policy-default auditd -y 
```

🔧 Enable SELinux
```sudo selinux-activate```

🔁 Reboot for SELinux to take effect
```sudo reboot```
```sestatus```

### 🧱 AppArmor

sudo aa-status
sudo apt install apparmor apparmor-utils -y
sudo aa-status





sudo apt install unattended-upgrades
sudo dpkg-reconfigure --priority=low unattended-upgrades


